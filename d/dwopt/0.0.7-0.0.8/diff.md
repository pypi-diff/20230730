# Comparing `tmp/dwopt-0.0.7.tar.gz` & `tmp/dwopt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwopt-0.0.7.tar", last modified: Tue Mar 21 12:27:09 2023, max compression
+gzip compressed data, was "dwopt-0.0.8.tar", last modified: Sun Jul 30 13:48:05 2023, max compression
```

## Comparing `dwopt-0.0.7.tar` & `dwopt-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-21 12:27:09.618433 dwopt-0.0.7/
--rw-r--r--   0 user      (1000) user      (1000)     1064 2023-03-20 10:32:27.000000 dwopt-0.0.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    16226 2023-03-21 12:27:09.618433 dwopt-0.0.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    15603 2023-03-21 12:22:22.000000 dwopt-0.0.7/README.rst
--rw-r--r--   0 user      (1000) user      (1000)      103 2023-03-20 06:20:06.000000 dwopt-0.0.7/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      784 2023-03-21 12:27:09.618433 dwopt-0.0.7/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-21 12:27:09.608433 dwopt-0.0.7/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-21 12:27:09.618433 dwopt-0.0.7/src/dwopt/
--rw-r--r--   0 user      (1000) user      (1000)      253 2023-03-20 06:20:06.000000 dwopt-0.0.7/src/dwopt/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    40630 2023-03-20 06:20:06.000000 dwopt-0.0.7/src/dwopt/_qry.py
--rw-r--r--   0 user      (1000) user      (1000)    41591 2023-03-20 10:32:27.000000 dwopt-0.0.7/src/dwopt/dbo.py
--rw-r--r--   0 user      (1000) user      (1000)    23209 2023-03-20 10:32:27.000000 dwopt-0.0.7/src/dwopt/set_up.py
--rw-r--r--   0 user      (1000) user      (1000)     8883 2023-03-20 10:32:27.000000 dwopt-0.0.7/src/dwopt/testing.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-21 12:27:09.618433 dwopt-0.0.7/src/dwopt.egg-info/
--rw-rw-rw-   0 user      (1000) user      (1000)    16226 2023-03-21 12:27:09.000000 dwopt-0.0.7/src/dwopt.egg-info/PKG-INFO
--rw-rw-rw-   0 user      (1000) user      (1000)      413 2023-03-21 12:27:09.000000 dwopt-0.0.7/src/dwopt.egg-info/SOURCES.txt
--rw-rw-rw-   0 user      (1000) user      (1000)        1 2023-03-21 12:27:09.000000 dwopt-0.0.7/src/dwopt.egg-info/dependency_links.txt
--rw-rw-rw-   0 user      (1000) user      (1000)       45 2023-03-21 12:27:09.000000 dwopt-0.0.7/src/dwopt.egg-info/requires.txt
--rw-rw-rw-   0 user      (1000) user      (1000)        6 2023-03-21 12:27:09.000000 dwopt-0.0.7/src/dwopt.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-21 12:27:09.618433 dwopt-0.0.7/tests/
--rw-r--r--   0 user      (1000) user      (1000)     3022 2023-03-20 10:32:27.000000 dwopt-0.0.7/tests/test_db_meta.py
--rw-r--r--   0 user      (1000) user      (1000)     6721 2023-03-20 06:20:06.000000 dwopt-0.0.7/tests/test_db_opt.py
--rw-r--r--   0 user      (1000) user      (1000)     3240 2023-03-20 06:20:06.000000 dwopt-0.0.7/tests/test_qry_cls.py
--rw-r--r--   0 user      (1000) user      (1000)     1680 2023-03-20 10:32:27.000000 dwopt-0.0.7/tests/test_qry_sum.py
--rw-r--r--   0 user      (1000) user      (1000)      778 2023-03-20 06:20:06.000000 dwopt-0.0.7/tests/test_set_up.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:48:05.384421 dwopt-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-07-28 05:42:01.000000 dwopt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    18360 2023-07-30 13:48:05.385421 dwopt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    17764 2023-07-30 13:42:19.000000 dwopt-0.0.8/README.rst
+-rw-rw-rw-   0        0        0      108 2023-07-28 05:42:01.000000 dwopt-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      780 2023-07-30 13:48:05.388423 dwopt-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 13:48:05.299422 dwopt-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 13:48:05.324437 dwopt-0.0.8/src/dwopt/
+-rw-rw-rw-   0        0        0      758 2023-07-30 13:42:19.000000 dwopt-0.0.8/src/dwopt/__init__.py
+-rw-rw-rw-   0        0        0    41947 2023-07-30 13:42:19.000000 dwopt-0.0.8/src/dwopt/_qry.py
+-rw-rw-rw-   0        0        0    43654 2023-07-30 13:42:19.000000 dwopt-0.0.8/src/dwopt/dbo.py
+-rw-rw-rw-   0        0        0    27283 2023-07-30 13:42:19.000000 dwopt-0.0.8/src/dwopt/set_up.py
+-rw-rw-rw-   0        0        0     9284 2023-07-30 13:42:19.000000 dwopt-0.0.8/src/dwopt/testing.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:48:05.358423 dwopt-0.0.8/src/dwopt.egg-info/
+-rw-rw-rw-   0        0        0    18360 2023-07-30 13:48:05.000000 dwopt-0.0.8/src/dwopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-07-30 13:48:05.000000 dwopt-0.0.8/src/dwopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 13:48:05.000000 dwopt-0.0.8/src/dwopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-30 13:48:05.000000 dwopt-0.0.8/src/dwopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 13:48:05.000000 dwopt-0.0.8/src/dwopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 13:48:05.383423 dwopt-0.0.8/tests/
+-rw-rw-rw-   0        0        0     3144 2023-07-28 05:42:01.000000 dwopt-0.0.8/tests/test_db_meta.py
+-rw-rw-rw-   0        0        0     6952 2023-07-30 13:42:19.000000 dwopt-0.0.8/tests/test_db_opt.py
+-rw-rw-rw-   0        0        0     3398 2023-07-30 13:42:19.000000 dwopt-0.0.8/tests/test_qry_cls.py
+-rw-rw-rw-   0        0        0     1756 2023-07-28 05:42:01.000000 dwopt-0.0.8/tests/test_qry_sum.py
+-rw-rw-rw-   0        0        0     1710 2023-07-30 13:42:19.000000 dwopt-0.0.8/tests/test_set_up.py
```

### Comparing `dwopt-0.0.7/PKG-INFO` & `dwopt-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,579 +1,636 @@
-Metadata-Version: 2.1
-Name: dwopt
-Version: 0.0.7
-Summary: Datawarehouse operator
-Home-page: https://github.com/0xdomyz/dwopt
-Author: 0xdomyz
-Author-email: septemberwhyms@gmail.com
-Project-URL: Bug Tracker, https://github.com/0xdomyz/dwopt/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-DWOPT - Datawarehouse Operator
-==============================
-
-Getting summary statistics out of database tables is often an unstreamlined process.
-Does one read in millions of rows before doing any work on Python,
-or run sql elsewhere and use intermediate CSVs,
-or write sql strings in python scripts?
-
-The Python package **dwopt**
-provides Excel-pivot-table-like and dataframe-summary-methods-like API,
-driven by sql templates, under a flexible summary query building framework.
-
-See the Features and the Walk Through section for examples.
-
-.. end-of-readme-intro
-
-
-Installation
-------------
-
-.. code-block:: console
-
-    pip install dwopt
-
-
-Features
---------
-
-* `Run sql frictionlessly using saved credentials`_
-* `Run sql script with text replacement`_
-* `Programatically make simple sql query`_
-* `Templates: Excel-pivot-table-like API`_
-* `Templates: Dataframe-summary-methods-like API`_
-* `Templates: DDL/DML statements, metadata queries`_
-* `Standard logging with reproducible sql`_
-
-
-Walk Through
-------------
-
-Run sql frictionlessly using saved credentials
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
-.. |dwopt.db| replace:: ``dwopt.db``
-.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
-.. |dwopt.save_url| replace:: ``dwopt.save_url``
-.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
-
-On import, the package gives ready-to-be-used `database operator objects`_
-with default credentials, which could be saved prior by user to
-the system keyring using the |dwopt.save_url|_ function.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.run('select count(1) from iris')
-       count
-    0    150
-
-This enable quick analysis from any Python/Console window:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.qry('iris').valc('species', 'avg(petal_length)')
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, use the database operator object factory function |dwopt.db|_
-and the database engine url to access database.
-
-.. code-block:: python
-
-    from dwopt import db
-    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
-    d.mtcars()
-    d.run('select count(1) n from mtcars')
-        n
-    0  32
-
-Supports:
-
-* Python 3.9, 3.10, 3.11.
-* Windows 10: Sqlite, Postgre, Oracle.
-* Linux: Sqlite, Postgre.
-
-See `Testing`_ section for package version tested.
-
-Run sql script with text replacement
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |run| replace:: ``run``
-.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
-
-Use the database operator object's
-|run|_ method to run sql script file.
-One could then replace ``:`` marked parameters via mappings supplied to the method.
-
-.. code-block:: python
-
-    from dwopt import pg, make_test_tbl
-    _ = make_test_tbl(pg)
-    pg.run(pth = "E:/projects/my_sql_script.sql",
-        my_run_dte = '2022-03-03',
-        my_label = '20220303',
-        threshold = 5)
-       count
-    0    137
-
-Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
-
-.. code-block:: sql
-
-    drop table if exists monthly_extract_:my_label;
-
-    create table monthly_extract_:my_label as
-    select * from test
-    where
-        dte = to_date(':my_run_dte','YYYY-MM-DD')
-        and score > :threshold;
-
-    select count(1) from monthly_extract_:my_label;
-
-
-Programatically make simple sql query
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
-.. |qry| replace:: ``qry``
-.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
-.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
-.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
-
-The database operator object's |qry|_ method returns the `query object`_.
-Use it's `list of clause methods`_ to make a simple sql query.
-
-This is not faster than just writing the sql,
-main usage is to provide flexibility to the `summary query building framework`_.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.mtcars()
-    sql = "select cyl from mtcars group by cyl having count(1) > 10"
-    q = (
-        lt.qry('mtcars a')
-        .select('a.cyl, count(1) n, avg(a.mpg)')
-        .case('cat', "a.cyl = 8 then 1", els=0)
-        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
-        .group_by('a.cyl')
-        .having('count(1) > 10')
-        .order_by('n desc')
-    )
-    q.run()
-       cyl   n  avg(a.mpg)  cat
-    0    8  14   15.100000    1
-    1    4  11   26.663636    0
-
-.. code-block:: sql
-
-    q.print()
-    select a.cyl, count(1) n, avg(a.mpg)
-        ,case when a.cyl = 8 then 1 else 0 end as cat
-    from mtcars a
-    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
-        on a.cyl = b.cyl
-    group by a.cyl
-    having count(1) > 10
-    order by n desc
-
-
-Templates: Excel-pivot-table-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |valc| replace:: ``valc``
-.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
-
-.. |pivot| replace:: ``pivot``
-.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
-
-Use the `query object`_ and it's |valc|_ method to make and run
-a value counts summary query with custom groups and calcs,
-on top of arbituary sub-query, as part of the `summary query building framework`_.
-
-Then call the result dataframe's |pivot|_ method to finalize the pivot table.
-
-.. code-block:: python
-
-    from dwopt import lt, make_test_tbl
-    _ = make_test_tbl(lt)
-    (
-        lt.qry('test')
-        .where('score>0.5', 'dte is not null', 'cat is not null')
-        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
-        .pivot('dte', 'cat')
-    )
-
-Result:
-
-==========  =====  =====  ========  ========  ======  ======
-cat           n           avgscore             total
-----------  -----  -----  --------  --------  ------  ------
-dte         test   train    test     train     test   train 
-==========  =====  =====  ========  ========  ======  ======
-2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
-2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
-2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
-==========  =====  =====  ========  ========  ======  ======
-
-The final query used can be invoked by the |valc|_ method, or logged via standard
-logging.
-
-.. code-block:: sql
-
-    with x as (
-        select * from test
-        where score>0.5
-            and dte is not null
-            and cat is not null
-    )
-    select
-        dte,cat
-        ,count(1) n
-        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
-    from x
-    group by dte,cat
-    order by n desc
-
-
-Templates: Dataframe-summary-methods-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
-
-Use the `query object`_ and it's `list of summary methods`_ to make and run
-summary queries on top of arbituary sub-query,
-as part of the `summary query building framework`_:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    q = pg.qry('iris a').select('a.*').case('cat',
-        "petal_length > 5             then '5+'",
-        "petal_length between 2 and 5 then '2-5'",
-        "petal_length < 2             then '-2'",
-    )
-
-    #Column names:
-    q.cols()
-    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
-
-    #Number of distinct combination:
-    q.dist(['species', 'petal_length'])
-    count    48
-    Name: 0, dtype: int64
-
-    #Head:
-    q.head()
-       sepal_length  sepal_width  petal_length  petal_width species cat
-    0           5.1          3.5           1.4          0.2  setosa  -2
-    1           4.9          3.0           1.4          0.2  setosa  -2
-    2           4.7          3.2           1.3          0.2  setosa  -2
-    3           4.6          3.1           1.5          0.2  setosa  -2
-    4           5.0          3.6           1.4          0.2  setosa  -2
-
-    #Length:
-    q.len()
-    150
-
-    #Min and max value:
-    q.mimx('petal_length')
-    max    6.9
-    min    1.0
-    Name: 0, dtype: float64
-
-    #Top record:
-    q.top()
-    sepal_length       5.1
-    sepal_width        3.5
-    petal_length       1.4
-    petal_width        0.2
-    species         setosa
-    cat                 -2
-    Name: 0, dtype: object
-
-    #Value count followed by pivot:
-    q.valc('species, cat').pivot('species','cat','n')
-    cat        -2   2-5    5+
-    species
-    rginica   NaN   9.0  41.0
-    setosa   50.0   NaN   NaN
-    sicolor   NaN  49.0   1.0
-
-.. code-block:: sql
-
-    #--All summary methods support output by printing or str:
-    q.valc('species, cat', out=1)
-    with x as (
-        select a.*
-            ,case
-                when petal_length > 5             then '5+'
-                when petal_length between 2 and 5 then '2-5'
-                when petal_length < 2             then '-2'
-                else NULL
-            end as cat
-        from iris a
-    )
-    select
-        species, cat
-        ,count(1) n
-    from x
-    group by species, cat
-    order by n desc
-
-Templates: DDL/DML statements, metadata queries
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
-.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
-
-Use the `list of operation methods`_ to make and run some
-DDL/DML statements with convenient or enhanced functionalities:
-
-.. code-block:: python
-
-    import pandas as pd
-    from dwopt import lt
-    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
-    lt.drop('test')
-    lt.create('test', col1='int', col2='text')
-    lt.write(tbl, 'test')
-    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
-    lt.run("select * from test")
-       col1 col2
-    0     1    a
-    1     2    b
-    2     3    c
-
-.. code-block:: python
-
-    lt.drop('test')
-    lt.cwrite(tbl, 'test')
-    lt.qry('test').run()
-       col1 col2
-    0     1    a
-    1     2    b
-
-
-Use the `list of metadata methods`_ to make and run some useful metadata queries:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.table_cols('public.iris')
-        column_name          data_type
-    0  sepal_length               real
-    1   sepal_width               real
-    2  petal_length               real
-    3   petal_width               real
-    4       species  character varying
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.mtcars()
-    lt.list_tables().iloc[:,:-1]
-        type    name tbl_name  rootpage
-    0  table    iris     iris         2
-    1  table  mtcars   mtcars         5
-
-
-Standard logging with reproducible sql
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |INFO| replace:: ``INFO``
-.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
-
-Many of the package's methods are wired through the standard
-`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
-package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
-The relevant logger object has standard naming and is called ``dwopt.dbo``.
-
-Example configuration to show logs in console:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(level = logging.INFO)
-
-    from dwopt import lt
-    lt.iris(q=1).valc('species', 'avg(petal_length)')
-
-.. code-block:: text
-
-    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:creating table via sqlalchemy:
-    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
-    INFO:dwopt.dbo:args len=150, e.g.
-    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    with x as (
-        select * from iris
-    )
-    select
-        species
-        ,count(1) n
-        ,avg(petal_length)
-    from x
-    group by species
-    order by n desc
-    INFO:dwopt.dbo:done
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, to avoid logging info messages from other packages:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Example configuration to print on console and store on file with timestamps:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(
-        format = "%(asctime)s [%(levelname)s] %(message)s"
-        ,handlers=[
-            logging.FileHandler("E:/projects/logs.log"),
-            logging.StreamHandler()
-        ]
-    )
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Sqlalchemy logger can also be used to obtain even more details:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
-
-
-Development
----------------
-
-Installation
-^^^^^^^^^^^^^^^
-
-Testing, documentation building package:
-
-.. code-block:: console
-
-    #testing
-    python -m pip install pytest black flake8 tox
-    
-    #doco and packaging
-    python -m pip install sphinx sphinx_rtd_theme build twine
-    
-    #depend
-    python -m pip install -U sqlalchemy psycopg2 cx_Oracle pandas keyring
-    
-    #package
-    python -m pip install -e .
-
-Testing
-^^^^^^^^^^^^
-
-Test:
-
-.. code-block:: console
-
-    python -m tox
-
-.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
-.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
-
-Testing for specific databases.
-Set up environment based on |dwopt.make_test_tbl|_ function notes.
-
-.. code-block:: console
-
-    python -m pytest
-    python -m pytest --db=pg
-    python -m pytest --db=oc
-
-Test code styles:
-
-.. code-block:: console
-
-    flake8 src/dwopt
-
-Package versions tested are::
-
-    Name: SQLAlchemy
-    Version: 2.0.7
-    ---
-    Name: psycopg2
-    Version: 2.9.5
-    ---
-    Name: cx-Oracle
-    Version: 8.3.0
-    ---
-    Name: pandas
-    Version: 1.5.3
-    ---
-    Name: keyring
-    Version: 23.13.1
-
-Documentation
-^^^^^^^^^^^^^^^^^
-
-Build document:
-
-.. code-block:: console
-
-    cd docs
-    make html
-
-Test examples across docs:
-
-.. code-block:: console
-
-    cd docs
-    make doctest
-
-Future
-^^^^^^^^^
-
-* For text replacement directives, use
-  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
-* Add more summary, DML/DDL, metadata templates.
-
-.. end-of-readme-usage
-
-
-Documentation
--------------
-
-* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
+Metadata-Version: 2.1
+Name: dwopt
+Version: 0.0.8
+Summary: SQL query abstraction library
+Home-page: https://github.com/0xdomyz/dwopt
+Author: 0xdomyz
+Author-email: septemberwhyms@gmail.com
+Project-URL: Bug Tracker, https://github.com/0xdomyz/dwopt/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+DWOPT - SQL query abstraction library
+========================================
+
+Getting summary statistics out of database tables is often an unstreamlined process.
+Does one read in millions of rows before doing any work on Python,
+or run SQL elsewhere and use intermediate CSVs,
+or write sql strings in python scripts?
+
+The Python package **dwopt** (Datawarehouse Operator)
+uses classes with a collection of sql templates to dynamically build and run queries,
+under a flexible summary query building framework.
+
+Specifically, it features Excel-pivot-table-like API,
+a collection of dataframe-summary-methods-like API,
+and a collection of DDL/DML statements, metadata query wrappers.
+
+Supports:
+
+* Python 3.10, 3.11.
+* Windows 10: Sqlite, Postgres, Oracle.
+* Linux: Sqlite, Postgres.
+
+See the Features and the Walk Through section for examples.
+
+.. end-of-readme-intro
+
+
+Installation
+------------
+
+.. code-block:: console
+
+    pip install dwopt
+
+Install the database drivers for the database engines you want to use.
+
+.. code-block:: console
+
+    pip install psycopg2 # postgres
+    pip install psycopg2-binary # in case can't build psycopg2
+    
+    pip install oracledb # oracle
+
+Features
+--------
+
+* `Run sql frictionlessly using saved credentials`_
+* `Run sql script with text replacement`_
+* `Programatically make simple sql query`_
+* `Templates: Excel-pivot-table-like API`_
+* `Templates: Dataframe-summary-methods-like API`_
+* `Templates: DDL/DML statements, metadata queries`_
+* `Standard logging with reproducible sql`_
+
+
+Walk Through
+------------
+
+Run sql frictionlessly using saved credentials
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
+.. |dwopt.db| replace:: ``dwopt.db``
+.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
+.. |dwopt.save_url| replace:: ``dwopt.save_url``
+.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
+
+On import, the package gives ready-to-be-used `database operator objects`_
+with default credentials, which could be saved prior by user to
+the system keyring using the |dwopt.save_url|_ function.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.run('select count(1) from iris')
+       count
+    0    150
+
+This enable quick analysis from any Python/Console window:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.qry('iris').valc('species', 'avg(petal_length)')
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, use the database operator object factory function |dwopt.db|_
+and the database engine url to access database.
+
+.. code-block:: python
+
+    from dwopt import db
+    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
+    d.mtcars()
+    d.run('select count(1) n from mtcars')
+        n
+    0  32
+
+Allows for thick mode connection to Oracle database:
+
+.. code-block:: python
+
+    from dwopt import db
+    url = """oracle+oracledb://dwopt_test:1234@localhost:1521/?service_name=XEPDB1 
+    &encoding=UTF-8&nencoding=UTF-8"""
+    lib_dir = "C:/app/{user_name}/product/21c/dbhomeXE/bin"
+    o = db(url, thick_mode={"lib_dir": lib_dir})
+    o.run("select * from dual")
+      dummy
+    0     X
+
+See `Testing`_ section for package version tested.
+
+Run sql script with text replacement
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |run| replace:: ``run``
+.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
+
+Use the database operator object's
+|run|_ method to run sql script file.
+One could then replace ``:`` marked parameters via mappings supplied to the method.
+
+Colon syntax is to be deprecated.
+A future version will use jinja2 syntax across the board.
+
+.. code-block:: python
+
+    from dwopt import pg, make_test_tbl
+    _ = make_test_tbl(pg)
+    pg.run(pth = "E:/projects/my_sql_script.sql",
+        my_run_dte = '2022-03-03',
+        my_label = '20220303',
+        threshold = 5)
+       count
+    0    137
+
+Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
+
+.. code-block:: sql
+
+    drop table if exists monthly_extract_:my_label;
+
+    create table monthly_extract_:my_label as
+    select * from test
+    where
+        dte = to_date(':my_run_dte','YYYY-MM-DD')
+        and score > :threshold;
+
+    select count(1) from monthly_extract_:my_label;
+
+
+Programatically make simple sql query
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
+.. |qry| replace:: ``qry``
+.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
+.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
+.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
+
+The database operator object's |qry|_ method returns the `query object`_.
+Use it's `list of clause methods`_ to make a simple sql query.
+
+This is not faster than just writing the sql,
+main usage is to provide flexibility to the `summary query building framework`_.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.mtcars()
+    sql = "select cyl from mtcars group by cyl having count(1) > 10"
+    q = (
+        lt.qry('mtcars a')
+        .select('a.cyl, count(1) n, avg(a.mpg)')
+        .case('cat', "a.cyl = 8 then 1", els=0)
+        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
+        .group_by('a.cyl')
+        .having('count(1) > 10')
+        .order_by('n desc')
+    )
+    q.run()
+       cyl   n  avg(a.mpg)  cat
+    0    8  14   15.100000    1
+    1    4  11   26.663636    0
+
+.. code-block:: sql
+
+    q.print()
+    select a.cyl, count(1) n, avg(a.mpg)
+        ,case when a.cyl = 8 then 1 else 0 end as cat
+    from mtcars a
+    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
+        on a.cyl = b.cyl
+    group by a.cyl
+    having count(1) > 10
+    order by n desc
+
+
+Templates: Excel-pivot-table-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |valc| replace:: ``valc``
+.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
+
+.. |pivot| replace:: ``pivot``
+.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
+
+Use the `query object`_ and it's |valc|_ method to make and run
+a value counts summary query with custom groups and calcs,
+on top of arbituary sub-query, as part of the `summary query building framework`_.
+
+Then call the result dataframe's |pivot|_ method to finalize the pivot table.
+
+.. code-block:: python
+
+    from dwopt import lt, make_test_tbl
+    _ = make_test_tbl(lt)
+    (
+        lt.qry('test')
+        .where('score>0.5', 'dte is not null', 'cat is not null')
+        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
+        .pivot('dte', 'cat')
+    )
+
+Result:
+
+==========  =====  =====  ========  ========  ======  ======
+cat           n           avgscore             total
+----------  -----  -----  --------  --------  ------  ------
+dte         test   train    test     train     test   train 
+==========  =====  =====  ========  ========  ======  ======
+2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
+2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
+2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
+==========  =====  =====  ========  ========  ======  ======
+
+The final query used can be invoked by the |valc|_ method, or logged via standard
+logging.
+
+.. code-block:: sql
+
+    with x as (
+        select * from test
+        where score>0.5
+            and dte is not null
+            and cat is not null
+    )
+    select
+        dte,cat
+        ,count(1) n
+        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
+    from x
+    group by dte,cat
+    order by n desc
+
+
+Templates: Dataframe-summary-methods-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
+
+Use the `query object`_ and it's `list of summary methods`_ to make and run
+summary queries on top of arbituary sub-query,
+as part of the `summary query building framework`_:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    q = pg.qry('iris a').select('a.*').case('cat',
+        "petal_length > 5             then '5+'",
+        "petal_length between 2 and 5 then '2-5'",
+        "petal_length < 2             then '-2'",
+    )
+
+    #Column names:
+    q.cols()
+    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
+
+    #Number of distinct combination:
+    q.dist(['species', 'petal_length'])
+    count    48
+    Name: 0, dtype: int64
+
+    #Head:
+    q.head()
+       sepal_length  sepal_width  petal_length  petal_width species cat
+    0           5.1          3.5           1.4          0.2  setosa  -2
+    1           4.9          3.0           1.4          0.2  setosa  -2
+    2           4.7          3.2           1.3          0.2  setosa  -2
+    3           4.6          3.1           1.5          0.2  setosa  -2
+    4           5.0          3.6           1.4          0.2  setosa  -2
+
+    #Length:
+    q.len()
+    150
+
+    #Min and max value:
+    q.mimx('petal_length')
+    max    6.9
+    min    1.0
+    Name: 0, dtype: float64
+
+    #Top record:
+    q.top()
+    sepal_length       5.1
+    sepal_width        3.5
+    petal_length       1.4
+    petal_width        0.2
+    species         setosa
+    cat                 -2
+    Name: 0, dtype: object
+
+    #Value count followed by pivot:
+    q.valc('species, cat').pivot('species','cat','n')
+    cat        -2   2-5    5+
+    species
+    rginica   NaN   9.0  41.0
+    setosa   50.0   NaN   NaN
+    sicolor   NaN  49.0   1.0
+
+.. code-block:: sql
+
+    #--All summary methods support output by printing or str:
+    q.valc('species, cat', out=1)
+    with x as (
+        select a.*
+            ,case
+                when petal_length > 5             then '5+'
+                when petal_length between 2 and 5 then '2-5'
+                when petal_length < 2             then '-2'
+                else NULL
+            end as cat
+        from iris a
+    )
+    select
+        species, cat
+        ,count(1) n
+    from x
+    group by species, cat
+    order by n desc
+
+Templates: DDL/DML statements, metadata queries
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
+.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
+
+Use the `list of operation methods`_ to make and run some
+DDL/DML statements with convenient or enhanced functionalities:
+
+.. code-block:: python
+
+    import pandas as pd
+    from dwopt import lt
+    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
+    lt.drop('test')
+    lt.create('test', col1='int', col2='text')
+    lt.write(tbl, 'test')
+    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
+    lt.run("select * from test")
+       col1 col2
+    0     1    a
+    1     2    b
+    2     3    c
+
+.. code-block:: python
+
+    lt.drop('test')
+    lt.cwrite(tbl, 'test')
+    lt.qry('test').run()
+       col1 col2
+    0     1    a
+    1     2    b
+
+
+Use the `list of metadata methods`_ to make and run some useful metadata queries:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.table_cols('public.iris')
+        column_name          data_type
+    0  sepal_length               real
+    1   sepal_width               real
+    2  petal_length               real
+    3   petal_width               real
+    4       species  character varying
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.mtcars()
+    lt.list_tables().iloc[:,:-1]
+        type    name tbl_name  rootpage
+    0  table    iris     iris         2
+    1  table  mtcars   mtcars         5
+
+
+Standard logging with reproducible sql
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |INFO| replace:: ``INFO``
+.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
+
+Many of the package's methods are wired through the standard
+`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
+package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
+The relevant logger object has standard naming and is called ``dwopt.dbo``.
+
+Example configuration to show logs in console:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(level = logging.INFO)
+
+    from dwopt import lt
+    lt.iris(q=1).valc('species', 'avg(petal_length)')
+
+.. code-block:: text
+
+    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:creating table via sqlalchemy:
+    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
+    INFO:dwopt.dbo:args len=150, e.g.
+    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    with x as (
+        select * from iris
+    )
+    select
+        species
+        ,count(1) n
+        ,avg(petal_length)
+    from x
+    group by species
+    order by n desc
+    INFO:dwopt.dbo:done
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, to avoid logging info messages from other packages:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Example configuration to print on console and store on file with timestamps:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(
+        format = "%(asctime)s [%(levelname)s] %(message)s"
+        ,handlers=[
+            logging.FileHandler("E:/projects/logs.log"),
+            logging.StreamHandler()
+        ]
+    )
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Debug logging:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt').setLevel(logging.DEBUG)
+
+Sqlalchemy logger can also be used to obtain even more details:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
+
+
+Development
+---------------
+
+Installation
+^^^^^^^^^^^^^^^
+
+Testing, documentation building package:
+
+.. code-block:: console
+
+    #venv on linux
+    sudo apt-get install python3-venv
+    python3.11 -m venv dwopt_dev
+    source dwopt_dev/bin/activate
+    deactivate
+
+    #testing
+    python -m pip install pytest black flake8 tox
+    
+    #doco and packaging
+    python -m pip install sphinx sphinx_rtd_theme build twine wheel
+    
+    #depend
+    python -m pip install -U sqlalchemy pandas keyring
+    python -m pip install -U keyrings.alt
+    python -m pip install -U psycopg2
+    python -m pip install -U oracledb
+    
+    #consider
+    python -m pip install -U psycopg2-binary
+    python -m pip install -U cx_Oracle
+    
+    #package
+    python -m pip install -e .
+
+Testing
+^^^^^^^^^^^^
+
+Test:
+
+.. code-block:: console
+
+    python -m tox
+
+.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
+.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
+
+Testing for specific databases.
+Set up environment based on |dwopt.make_test_tbl|_ function notes.
+
+.. code-block:: console
+
+    python -m pytest
+    python -m pytest --db=pg
+    python -m pytest --db=oc
+
+Test code styles:
+
+.. code-block:: console
+
+    flake8 src/dwopt
+
+Databases used for testings are::
+
+    Postgres 15
+    Oracle express 21c
+
+Package versions tested are::
+
+    Name: keyring
+    Version: 24.2.0
+    ---
+    Name: keyrings.alt
+    Version: 5.0.0
+    ---
+    Name: oracledb
+    Version: 1.3.2
+    ---
+    Name: pandas
+    Version: 2.0.3
+    ---
+    Name: psycopg2-binary
+    Version: 2.9.6
+    ---
+    Name: SQLAlchemy
+    Version: 2.0.19
+
+
+Documentation
+^^^^^^^^^^^^^^^^^
+
+Build document:
+
+.. code-block:: console
+
+    cd docs
+    make html
+
+Test examples across docs:
+
+.. code-block:: console
+
+    cd docs
+    make doctest
+
+Future
+^^^^^^^^^
+
+* For text replacement directives, use
+  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
+* Add more summary, DML/DDL, metadata templates.
+
+.. end-of-readme-usage
+
+
+Documentation
+-------------
+
+* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
```

### Comparing `dwopt-0.0.7/README.rst` & `dwopt-0.0.8/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,562 +1,620 @@
-DWOPT - Datawarehouse Operator
-==============================
-
-Getting summary statistics out of database tables is often an unstreamlined process.
-Does one read in millions of rows before doing any work on Python,
-or run sql elsewhere and use intermediate CSVs,
-or write sql strings in python scripts?
-
-The Python package **dwopt**
-provides Excel-pivot-table-like and dataframe-summary-methods-like API,
-driven by sql templates, under a flexible summary query building framework.
-
-See the Features and the Walk Through section for examples.
-
-.. end-of-readme-intro
-
-
-Installation
-------------
-
-.. code-block:: console
-
-    pip install dwopt
-
-
-Features
---------
-
-* `Run sql frictionlessly using saved credentials`_
-* `Run sql script with text replacement`_
-* `Programatically make simple sql query`_
-* `Templates: Excel-pivot-table-like API`_
-* `Templates: Dataframe-summary-methods-like API`_
-* `Templates: DDL/DML statements, metadata queries`_
-* `Standard logging with reproducible sql`_
-
-
-Walk Through
-------------
-
-Run sql frictionlessly using saved credentials
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
-.. |dwopt.db| replace:: ``dwopt.db``
-.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
-.. |dwopt.save_url| replace:: ``dwopt.save_url``
-.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
-
-On import, the package gives ready-to-be-used `database operator objects`_
-with default credentials, which could be saved prior by user to
-the system keyring using the |dwopt.save_url|_ function.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.run('select count(1) from iris')
-       count
-    0    150
-
-This enable quick analysis from any Python/Console window:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.qry('iris').valc('species', 'avg(petal_length)')
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, use the database operator object factory function |dwopt.db|_
-and the database engine url to access database.
-
-.. code-block:: python
-
-    from dwopt import db
-    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
-    d.mtcars()
-    d.run('select count(1) n from mtcars')
-        n
-    0  32
-
-Supports:
-
-* Python 3.9, 3.10, 3.11.
-* Windows 10: Sqlite, Postgre, Oracle.
-* Linux: Sqlite, Postgre.
-
-See `Testing`_ section for package version tested.
-
-Run sql script with text replacement
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |run| replace:: ``run``
-.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
-
-Use the database operator object's
-|run|_ method to run sql script file.
-One could then replace ``:`` marked parameters via mappings supplied to the method.
-
-.. code-block:: python
-
-    from dwopt import pg, make_test_tbl
-    _ = make_test_tbl(pg)
-    pg.run(pth = "E:/projects/my_sql_script.sql",
-        my_run_dte = '2022-03-03',
-        my_label = '20220303',
-        threshold = 5)
-       count
-    0    137
-
-Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
-
-.. code-block:: sql
-
-    drop table if exists monthly_extract_:my_label;
-
-    create table monthly_extract_:my_label as
-    select * from test
-    where
-        dte = to_date(':my_run_dte','YYYY-MM-DD')
-        and score > :threshold;
-
-    select count(1) from monthly_extract_:my_label;
-
-
-Programatically make simple sql query
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
-.. |qry| replace:: ``qry``
-.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
-.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
-.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
-
-The database operator object's |qry|_ method returns the `query object`_.
-Use it's `list of clause methods`_ to make a simple sql query.
-
-This is not faster than just writing the sql,
-main usage is to provide flexibility to the `summary query building framework`_.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.mtcars()
-    sql = "select cyl from mtcars group by cyl having count(1) > 10"
-    q = (
-        lt.qry('mtcars a')
-        .select('a.cyl, count(1) n, avg(a.mpg)')
-        .case('cat', "a.cyl = 8 then 1", els=0)
-        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
-        .group_by('a.cyl')
-        .having('count(1) > 10')
-        .order_by('n desc')
-    )
-    q.run()
-       cyl   n  avg(a.mpg)  cat
-    0    8  14   15.100000    1
-    1    4  11   26.663636    0
-
-.. code-block:: sql
-
-    q.print()
-    select a.cyl, count(1) n, avg(a.mpg)
-        ,case when a.cyl = 8 then 1 else 0 end as cat
-    from mtcars a
-    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
-        on a.cyl = b.cyl
-    group by a.cyl
-    having count(1) > 10
-    order by n desc
-
-
-Templates: Excel-pivot-table-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |valc| replace:: ``valc``
-.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
-
-.. |pivot| replace:: ``pivot``
-.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
-
-Use the `query object`_ and it's |valc|_ method to make and run
-a value counts summary query with custom groups and calcs,
-on top of arbituary sub-query, as part of the `summary query building framework`_.
-
-Then call the result dataframe's |pivot|_ method to finalize the pivot table.
-
-.. code-block:: python
-
-    from dwopt import lt, make_test_tbl
-    _ = make_test_tbl(lt)
-    (
-        lt.qry('test')
-        .where('score>0.5', 'dte is not null', 'cat is not null')
-        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
-        .pivot('dte', 'cat')
-    )
-
-Result:
-
-==========  =====  =====  ========  ========  ======  ======
-cat           n           avgscore             total
-----------  -----  -----  --------  --------  ------  ------
-dte         test   train    test     train     test   train 
-==========  =====  =====  ========  ========  ======  ======
-2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
-2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
-2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
-==========  =====  =====  ========  ========  ======  ======
-
-The final query used can be invoked by the |valc|_ method, or logged via standard
-logging.
-
-.. code-block:: sql
-
-    with x as (
-        select * from test
-        where score>0.5
-            and dte is not null
-            and cat is not null
-    )
-    select
-        dte,cat
-        ,count(1) n
-        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
-    from x
-    group by dte,cat
-    order by n desc
-
-
-Templates: Dataframe-summary-methods-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
-
-Use the `query object`_ and it's `list of summary methods`_ to make and run
-summary queries on top of arbituary sub-query,
-as part of the `summary query building framework`_:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    q = pg.qry('iris a').select('a.*').case('cat',
-        "petal_length > 5             then '5+'",
-        "petal_length between 2 and 5 then '2-5'",
-        "petal_length < 2             then '-2'",
-    )
-
-    #Column names:
-    q.cols()
-    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
-
-    #Number of distinct combination:
-    q.dist(['species', 'petal_length'])
-    count    48
-    Name: 0, dtype: int64
-
-    #Head:
-    q.head()
-       sepal_length  sepal_width  petal_length  petal_width species cat
-    0           5.1          3.5           1.4          0.2  setosa  -2
-    1           4.9          3.0           1.4          0.2  setosa  -2
-    2           4.7          3.2           1.3          0.2  setosa  -2
-    3           4.6          3.1           1.5          0.2  setosa  -2
-    4           5.0          3.6           1.4          0.2  setosa  -2
-
-    #Length:
-    q.len()
-    150
-
-    #Min and max value:
-    q.mimx('petal_length')
-    max    6.9
-    min    1.0
-    Name: 0, dtype: float64
-
-    #Top record:
-    q.top()
-    sepal_length       5.1
-    sepal_width        3.5
-    petal_length       1.4
-    petal_width        0.2
-    species         setosa
-    cat                 -2
-    Name: 0, dtype: object
-
-    #Value count followed by pivot:
-    q.valc('species, cat').pivot('species','cat','n')
-    cat        -2   2-5    5+
-    species
-    rginica   NaN   9.0  41.0
-    setosa   50.0   NaN   NaN
-    sicolor   NaN  49.0   1.0
-
-.. code-block:: sql
-
-    #--All summary methods support output by printing or str:
-    q.valc('species, cat', out=1)
-    with x as (
-        select a.*
-            ,case
-                when petal_length > 5             then '5+'
-                when petal_length between 2 and 5 then '2-5'
-                when petal_length < 2             then '-2'
-                else NULL
-            end as cat
-        from iris a
-    )
-    select
-        species, cat
-        ,count(1) n
-    from x
-    group by species, cat
-    order by n desc
-
-Templates: DDL/DML statements, metadata queries
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
-.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
-
-Use the `list of operation methods`_ to make and run some
-DDL/DML statements with convenient or enhanced functionalities:
-
-.. code-block:: python
-
-    import pandas as pd
-    from dwopt import lt
-    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
-    lt.drop('test')
-    lt.create('test', col1='int', col2='text')
-    lt.write(tbl, 'test')
-    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
-    lt.run("select * from test")
-       col1 col2
-    0     1    a
-    1     2    b
-    2     3    c
-
-.. code-block:: python
-
-    lt.drop('test')
-    lt.cwrite(tbl, 'test')
-    lt.qry('test').run()
-       col1 col2
-    0     1    a
-    1     2    b
-
-
-Use the `list of metadata methods`_ to make and run some useful metadata queries:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.table_cols('public.iris')
-        column_name          data_type
-    0  sepal_length               real
-    1   sepal_width               real
-    2  petal_length               real
-    3   petal_width               real
-    4       species  character varying
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.mtcars()
-    lt.list_tables().iloc[:,:-1]
-        type    name tbl_name  rootpage
-    0  table    iris     iris         2
-    1  table  mtcars   mtcars         5
-
-
-Standard logging with reproducible sql
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |INFO| replace:: ``INFO``
-.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
-
-Many of the package's methods are wired through the standard
-`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
-package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
-The relevant logger object has standard naming and is called ``dwopt.dbo``.
-
-Example configuration to show logs in console:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(level = logging.INFO)
-
-    from dwopt import lt
-    lt.iris(q=1).valc('species', 'avg(petal_length)')
-
-.. code-block:: text
-
-    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:creating table via sqlalchemy:
-    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
-    INFO:dwopt.dbo:args len=150, e.g.
-    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    with x as (
-        select * from iris
-    )
-    select
-        species
-        ,count(1) n
-        ,avg(petal_length)
-    from x
-    group by species
-    order by n desc
-    INFO:dwopt.dbo:done
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, to avoid logging info messages from other packages:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Example configuration to print on console and store on file with timestamps:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(
-        format = "%(asctime)s [%(levelname)s] %(message)s"
-        ,handlers=[
-            logging.FileHandler("E:/projects/logs.log"),
-            logging.StreamHandler()
-        ]
-    )
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Sqlalchemy logger can also be used to obtain even more details:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
-
-
-Development
----------------
-
-Installation
-^^^^^^^^^^^^^^^
-
-Testing, documentation building package:
-
-.. code-block:: console
-
-    #testing
-    python -m pip install pytest black flake8 tox
-    
-    #doco and packaging
-    python -m pip install sphinx sphinx_rtd_theme build twine
-    
-    #depend
-    python -m pip install -U sqlalchemy psycopg2 cx_Oracle pandas keyring
-    
-    #package
-    python -m pip install -e .
-
-Testing
-^^^^^^^^^^^^
-
-Test:
-
-.. code-block:: console
-
-    python -m tox
-
-.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
-.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
-
-Testing for specific databases.
-Set up environment based on |dwopt.make_test_tbl|_ function notes.
-
-.. code-block:: console
-
-    python -m pytest
-    python -m pytest --db=pg
-    python -m pytest --db=oc
-
-Test code styles:
-
-.. code-block:: console
-
-    flake8 src/dwopt
-
-Package versions tested are::
-
-    Name: SQLAlchemy
-    Version: 2.0.7
-    ---
-    Name: psycopg2
-    Version: 2.9.5
-    ---
-    Name: cx-Oracle
-    Version: 8.3.0
-    ---
-    Name: pandas
-    Version: 1.5.3
-    ---
-    Name: keyring
-    Version: 23.13.1
-
-Documentation
-^^^^^^^^^^^^^^^^^
-
-Build document:
-
-.. code-block:: console
-
-    cd docs
-    make html
-
-Test examples across docs:
-
-.. code-block:: console
-
-    cd docs
-    make doctest
-
-Future
-^^^^^^^^^
-
-* For text replacement directives, use
-  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
-* Add more summary, DML/DDL, metadata templates.
-
-.. end-of-readme-usage
-
-
-Documentation
--------------
-
-* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
+DWOPT - SQL query abstraction library
+========================================
+
+Getting summary statistics out of database tables is often an unstreamlined process.
+Does one read in millions of rows before doing any work on Python,
+or run SQL elsewhere and use intermediate CSVs,
+or write sql strings in python scripts?
+
+The Python package **dwopt** (Datawarehouse Operator)
+uses classes with a collection of sql templates to dynamically build and run queries,
+under a flexible summary query building framework.
+
+Specifically, it features Excel-pivot-table-like API,
+a collection of dataframe-summary-methods-like API,
+and a collection of DDL/DML statements, metadata query wrappers.
+
+Supports:
+
+* Python 3.10, 3.11.
+* Windows 10: Sqlite, Postgres, Oracle.
+* Linux: Sqlite, Postgres.
+
+See the Features and the Walk Through section for examples.
+
+.. end-of-readme-intro
+
+
+Installation
+------------
+
+.. code-block:: console
+
+    pip install dwopt
+
+Install the database drivers for the database engines you want to use.
+
+.. code-block:: console
+
+    pip install psycopg2 # postgres
+    pip install psycopg2-binary # in case can't build psycopg2
+    
+    pip install oracledb # oracle
+
+Features
+--------
+
+* `Run sql frictionlessly using saved credentials`_
+* `Run sql script with text replacement`_
+* `Programatically make simple sql query`_
+* `Templates: Excel-pivot-table-like API`_
+* `Templates: Dataframe-summary-methods-like API`_
+* `Templates: DDL/DML statements, metadata queries`_
+* `Standard logging with reproducible sql`_
+
+
+Walk Through
+------------
+
+Run sql frictionlessly using saved credentials
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
+.. |dwopt.db| replace:: ``dwopt.db``
+.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
+.. |dwopt.save_url| replace:: ``dwopt.save_url``
+.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
+
+On import, the package gives ready-to-be-used `database operator objects`_
+with default credentials, which could be saved prior by user to
+the system keyring using the |dwopt.save_url|_ function.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.run('select count(1) from iris')
+       count
+    0    150
+
+This enable quick analysis from any Python/Console window:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.qry('iris').valc('species', 'avg(petal_length)')
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, use the database operator object factory function |dwopt.db|_
+and the database engine url to access database.
+
+.. code-block:: python
+
+    from dwopt import db
+    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
+    d.mtcars()
+    d.run('select count(1) n from mtcars')
+        n
+    0  32
+
+Allows for thick mode connection to Oracle database:
+
+.. code-block:: python
+
+    from dwopt import db
+    url = """oracle+oracledb://dwopt_test:1234@localhost:1521/?service_name=XEPDB1 
+    &encoding=UTF-8&nencoding=UTF-8"""
+    lib_dir = "C:/app/{user_name}/product/21c/dbhomeXE/bin"
+    o = db(url, thick_mode={"lib_dir": lib_dir})
+    o.run("select * from dual")
+      dummy
+    0     X
+
+See `Testing`_ section for package version tested.
+
+Run sql script with text replacement
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |run| replace:: ``run``
+.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
+
+Use the database operator object's
+|run|_ method to run sql script file.
+One could then replace ``:`` marked parameters via mappings supplied to the method.
+
+Colon syntax is to be deprecated.
+A future version will use jinja2 syntax across the board.
+
+.. code-block:: python
+
+    from dwopt import pg, make_test_tbl
+    _ = make_test_tbl(pg)
+    pg.run(pth = "E:/projects/my_sql_script.sql",
+        my_run_dte = '2022-03-03',
+        my_label = '20220303',
+        threshold = 5)
+       count
+    0    137
+
+Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
+
+.. code-block:: sql
+
+    drop table if exists monthly_extract_:my_label;
+
+    create table monthly_extract_:my_label as
+    select * from test
+    where
+        dte = to_date(':my_run_dte','YYYY-MM-DD')
+        and score > :threshold;
+
+    select count(1) from monthly_extract_:my_label;
+
+
+Programatically make simple sql query
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
+.. |qry| replace:: ``qry``
+.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
+.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
+.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
+
+The database operator object's |qry|_ method returns the `query object`_.
+Use it's `list of clause methods`_ to make a simple sql query.
+
+This is not faster than just writing the sql,
+main usage is to provide flexibility to the `summary query building framework`_.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.mtcars()
+    sql = "select cyl from mtcars group by cyl having count(1) > 10"
+    q = (
+        lt.qry('mtcars a')
+        .select('a.cyl, count(1) n, avg(a.mpg)')
+        .case('cat', "a.cyl = 8 then 1", els=0)
+        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
+        .group_by('a.cyl')
+        .having('count(1) > 10')
+        .order_by('n desc')
+    )
+    q.run()
+       cyl   n  avg(a.mpg)  cat
+    0    8  14   15.100000    1
+    1    4  11   26.663636    0
+
+.. code-block:: sql
+
+    q.print()
+    select a.cyl, count(1) n, avg(a.mpg)
+        ,case when a.cyl = 8 then 1 else 0 end as cat
+    from mtcars a
+    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
+        on a.cyl = b.cyl
+    group by a.cyl
+    having count(1) > 10
+    order by n desc
+
+
+Templates: Excel-pivot-table-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |valc| replace:: ``valc``
+.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
+
+.. |pivot| replace:: ``pivot``
+.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
+
+Use the `query object`_ and it's |valc|_ method to make and run
+a value counts summary query with custom groups and calcs,
+on top of arbituary sub-query, as part of the `summary query building framework`_.
+
+Then call the result dataframe's |pivot|_ method to finalize the pivot table.
+
+.. code-block:: python
+
+    from dwopt import lt, make_test_tbl
+    _ = make_test_tbl(lt)
+    (
+        lt.qry('test')
+        .where('score>0.5', 'dte is not null', 'cat is not null')
+        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
+        .pivot('dte', 'cat')
+    )
+
+Result:
+
+==========  =====  =====  ========  ========  ======  ======
+cat           n           avgscore             total
+----------  -----  -----  --------  --------  ------  ------
+dte         test   train    test     train     test   train 
+==========  =====  =====  ========  ========  ======  ======
+2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
+2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
+2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
+==========  =====  =====  ========  ========  ======  ======
+
+The final query used can be invoked by the |valc|_ method, or logged via standard
+logging.
+
+.. code-block:: sql
+
+    with x as (
+        select * from test
+        where score>0.5
+            and dte is not null
+            and cat is not null
+    )
+    select
+        dte,cat
+        ,count(1) n
+        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
+    from x
+    group by dte,cat
+    order by n desc
+
+
+Templates: Dataframe-summary-methods-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
+
+Use the `query object`_ and it's `list of summary methods`_ to make and run
+summary queries on top of arbituary sub-query,
+as part of the `summary query building framework`_:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    q = pg.qry('iris a').select('a.*').case('cat',
+        "petal_length > 5             then '5+'",
+        "petal_length between 2 and 5 then '2-5'",
+        "petal_length < 2             then '-2'",
+    )
+
+    #Column names:
+    q.cols()
+    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
+
+    #Number of distinct combination:
+    q.dist(['species', 'petal_length'])
+    count    48
+    Name: 0, dtype: int64
+
+    #Head:
+    q.head()
+       sepal_length  sepal_width  petal_length  petal_width species cat
+    0           5.1          3.5           1.4          0.2  setosa  -2
+    1           4.9          3.0           1.4          0.2  setosa  -2
+    2           4.7          3.2           1.3          0.2  setosa  -2
+    3           4.6          3.1           1.5          0.2  setosa  -2
+    4           5.0          3.6           1.4          0.2  setosa  -2
+
+    #Length:
+    q.len()
+    150
+
+    #Min and max value:
+    q.mimx('petal_length')
+    max    6.9
+    min    1.0
+    Name: 0, dtype: float64
+
+    #Top record:
+    q.top()
+    sepal_length       5.1
+    sepal_width        3.5
+    petal_length       1.4
+    petal_width        0.2
+    species         setosa
+    cat                 -2
+    Name: 0, dtype: object
+
+    #Value count followed by pivot:
+    q.valc('species, cat').pivot('species','cat','n')
+    cat        -2   2-5    5+
+    species
+    rginica   NaN   9.0  41.0
+    setosa   50.0   NaN   NaN
+    sicolor   NaN  49.0   1.0
+
+.. code-block:: sql
+
+    #--All summary methods support output by printing or str:
+    q.valc('species, cat', out=1)
+    with x as (
+        select a.*
+            ,case
+                when petal_length > 5             then '5+'
+                when petal_length between 2 and 5 then '2-5'
+                when petal_length < 2             then '-2'
+                else NULL
+            end as cat
+        from iris a
+    )
+    select
+        species, cat
+        ,count(1) n
+    from x
+    group by species, cat
+    order by n desc
+
+Templates: DDL/DML statements, metadata queries
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
+.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
+
+Use the `list of operation methods`_ to make and run some
+DDL/DML statements with convenient or enhanced functionalities:
+
+.. code-block:: python
+
+    import pandas as pd
+    from dwopt import lt
+    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
+    lt.drop('test')
+    lt.create('test', col1='int', col2='text')
+    lt.write(tbl, 'test')
+    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
+    lt.run("select * from test")
+       col1 col2
+    0     1    a
+    1     2    b
+    2     3    c
+
+.. code-block:: python
+
+    lt.drop('test')
+    lt.cwrite(tbl, 'test')
+    lt.qry('test').run()
+       col1 col2
+    0     1    a
+    1     2    b
+
+
+Use the `list of metadata methods`_ to make and run some useful metadata queries:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.table_cols('public.iris')
+        column_name          data_type
+    0  sepal_length               real
+    1   sepal_width               real
+    2  petal_length               real
+    3   petal_width               real
+    4       species  character varying
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.mtcars()
+    lt.list_tables().iloc[:,:-1]
+        type    name tbl_name  rootpage
+    0  table    iris     iris         2
+    1  table  mtcars   mtcars         5
+
+
+Standard logging with reproducible sql
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |INFO| replace:: ``INFO``
+.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
+
+Many of the package's methods are wired through the standard
+`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
+package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
+The relevant logger object has standard naming and is called ``dwopt.dbo``.
+
+Example configuration to show logs in console:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(level = logging.INFO)
+
+    from dwopt import lt
+    lt.iris(q=1).valc('species', 'avg(petal_length)')
+
+.. code-block:: text
+
+    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:creating table via sqlalchemy:
+    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
+    INFO:dwopt.dbo:args len=150, e.g.
+    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    with x as (
+        select * from iris
+    )
+    select
+        species
+        ,count(1) n
+        ,avg(petal_length)
+    from x
+    group by species
+    order by n desc
+    INFO:dwopt.dbo:done
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, to avoid logging info messages from other packages:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Example configuration to print on console and store on file with timestamps:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(
+        format = "%(asctime)s [%(levelname)s] %(message)s"
+        ,handlers=[
+            logging.FileHandler("E:/projects/logs.log"),
+            logging.StreamHandler()
+        ]
+    )
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Debug logging:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt').setLevel(logging.DEBUG)
+
+Sqlalchemy logger can also be used to obtain even more details:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
+
+
+Development
+---------------
+
+Installation
+^^^^^^^^^^^^^^^
+
+Testing, documentation building package:
+
+.. code-block:: console
+
+    #venv on linux
+    sudo apt-get install python3-venv
+    python3.11 -m venv dwopt_dev
+    source dwopt_dev/bin/activate
+    deactivate
+
+    #testing
+    python -m pip install pytest black flake8 tox
+    
+    #doco and packaging
+    python -m pip install sphinx sphinx_rtd_theme build twine wheel
+    
+    #depend
+    python -m pip install -U sqlalchemy pandas keyring
+    python -m pip install -U keyrings.alt
+    python -m pip install -U psycopg2
+    python -m pip install -U oracledb
+    
+    #consider
+    python -m pip install -U psycopg2-binary
+    python -m pip install -U cx_Oracle
+    
+    #package
+    python -m pip install -e .
+
+Testing
+^^^^^^^^^^^^
+
+Test:
+
+.. code-block:: console
+
+    python -m tox
+
+.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
+.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
+
+Testing for specific databases.
+Set up environment based on |dwopt.make_test_tbl|_ function notes.
+
+.. code-block:: console
+
+    python -m pytest
+    python -m pytest --db=pg
+    python -m pytest --db=oc
+
+Test code styles:
+
+.. code-block:: console
+
+    flake8 src/dwopt
+
+Databases used for testings are::
+
+    Postgres 15
+    Oracle express 21c
+
+Package versions tested are::
+
+    Name: keyring
+    Version: 24.2.0
+    ---
+    Name: keyrings.alt
+    Version: 5.0.0
+    ---
+    Name: oracledb
+    Version: 1.3.2
+    ---
+    Name: pandas
+    Version: 2.0.3
+    ---
+    Name: psycopg2-binary
+    Version: 2.9.6
+    ---
+    Name: SQLAlchemy
+    Version: 2.0.19
+
+
+Documentation
+^^^^^^^^^^^^^^^^^
+
+Build document:
+
+.. code-block:: console
+
+    cd docs
+    make html
+
+Test examples across docs:
+
+.. code-block:: console
+
+    cd docs
+    make doctest
+
+Future
+^^^^^^^^^
+
+* For text replacement directives, use
+  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
+* Add more summary, DML/DDL, metadata templates.
+
+.. end-of-readme-usage
+
+
+Documentation
+-------------
+
+* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
```

### Comparing `dwopt-0.0.7/src/dwopt/_qry.py` & `dwopt-0.0.8/src/dwopt/_qry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1355 +1,1353 @@
-import pandas as pd
-
-
-class _Qry:
-    """
-    The query class.
-
-    See examples for quick-start.
-
-    Automatically instantiated via the :meth:`~dwopt.dbo._Db.qry` method from the
-    :class:`database operator <dwopt.dbo._Db>` objects.
-
-    It is possible to pass in all needed parameters when calling the method.
-    But it is clearer to only pass in one positional argument as table name,
-    and use the :ref:`clause methods` to build up a query instead.
-
-    Parameters
-    ----------
-    operator : dwopt.db._Db
-        Database operator object to operate on generated queries.
-    from_ : str
-        Query table name.
-    select: str
-        Columns.
-    join : str
-        Join clause.
-    where : str
-        Conditions.
-    group_by : str
-        Group by names.
-    having : str
-        Conditions.
-    order_by : str
-        Order by names.
-    sql : str
-        Sql code.
-
-    Notes
-    -----
-    .. _The summary query building framework:
-
-    **The summary query building framework**
-
-    Queries are flexibly built as a combination of a ``sub query``
-    and a ``summary query`` from templates.
-    Point of ``sub query`` is to be a flexible complementary pre-processing step,
-    productivity gain comes from the ``summary query`` templates.
-
-    Example:
-
-    .. code-block:: sql
-
-        -- Sub query: arbituary query within a with clause named x
-        with x as (
-            select * from test
-            where score>0.5
-                and dte is not null
-                and cat is not null
-        )
-        -- Summary query: generated from templates
-        select
-            dte, cat
-            ,count(1) n
-            ,avg(score) avgscore, round(sum(amt)/1e3,2) total
-        from x
-        group by dte, cat
-        order by n desc
-
-    Corresponding code::
-
-        from dwopt import lt, make_test_tbl
-        _ = make_test_tbl(lt)
-        (
-            lt.qry('test').where('score>0.5', 'dte is not null', 'cat is not null')
-            .valc(
-                'dte, cat',
-                'avg(score) avgscore, round(sum(amt)/1e3,2) total',
-                out=1
-            )
-        )
-
-    Use the :ref:`clause methods` to iteratively
-    piece together a query, or use the :meth:`~dwopt._qry._Qry.sql` method to provide
-    an arbituary query. This created query will then be placed inside a
-    with block and become the ``sub query`` on invocation of any summary methods.
-
-    The ``summary query`` is built from parameterized templates via
-    the :ref:`summary methods`. Calling one of them completes the whole query
-    and immediately runs it.
-
-    This way for large tables, heavy intermediate results from the ``sub query``
-    are never realized outside of the database engine,
-    while light summary results are placed in python for analysis.
-
-    Examples
-    --------
-
-    Create and use qry object using the :meth:`~dwopt.dbo._Db.qry` method from the
-    :class:`database operator <dwopt.dbo._Db>` objects:
-
-    >>> from dwopt import lt
-    >>> lt.iris()
-    >>> lt.qry('iris').len()
-    150
-    >>> lt.qry('iris').valc('species', 'avg(petal_length)')
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-    >>> lt.qry('iris').where('petal_length > 2').valc('species', out=1)# doctest: +SKIP
-    with x as (
-        select * from iris
-        where petal_length > 2
-    )
-    select
-        species
-        ,count(1) n
-    from x
-    group by species
-    order by n desc
-
-    Iteratively piece together a query using the :ref:`clause methods`:
-
-    >>> from dwopt import lt
-    >>> lt.mtcars()
-    >>> sql = "select cyl from mtcars group by cyl having count(1) > 10"
-    >>> q = (
-    ...     lt.qry('mtcars a')
-    ...     .select('a.cyl, count(1) n, avg(a.mpg)')
-    ...     .case('cat', "a.cyl = 8 then 1", els=0)
-    ...     .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
-    ...     .group_by('a.cyl')
-    ...     .having('count(1) > 10')
-    ...     .order_by('n desc')
-    ... )
-    >>>
-    >>> q.print()
-    select a.cyl, count(1) n, avg(a.mpg)
-        ,case when a.cyl = 8 then 1 else 0 end as cat
-    from mtcars a
-    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
-        on a.cyl = b.cyl
-    group by a.cyl
-    having count(1) > 10
-    order by n desc
-    >>> q.run()
-       cyl   n  avg(a.mpg)  cat
-    0    8  14   15.100000    1
-    1    4  11   26.663636    0
-
-    Use the :ref:`summary methods` for analysis:
-
-    >>> from dwopt import pg as d
-    >>> d.iris('iris')
-    >>> q = d.qry('iris').where('petal_length > 2')
-    >>> q.top()
-    sepal_length        7.0
-    sepal_width         3.2
-    petal_length        4.7
-    petal_width         1.4
-    species         sicolor
-    Name: 0, dtype: object
-    >>> q.head()
-       sepal_length  sepal_width  petal_length  petal_width  species
-    0           7.0          3.2           4.7          1.4  sicolor
-    1           6.4          3.2           4.5          1.5  sicolor
-    2           6.9          3.1           4.9          1.5  sicolor
-    3           5.5          2.3           4.0          1.3  sicolor
-    4           6.5          2.8           4.6          1.5  sicolor
-    >>> q.len()
-    100
-    >>> agg = ', '.join(f'avg({col}) {col}' for col in q.cols() if col != 'species')
-    >>> q.valc('species', agg)
-       species   n  sepal_length  sepal_width  petal_length  petal_width
-    0  sicolor  50         5.936        2.770         4.260        1.326
-    1  rginica  50         6.588        2.974         5.552        2.026
-    """
-
-    def __init__(
-        self,
-        operator,
-        from_=None,
-        select=None,
-        join=None,
-        where=None,
-        group_by=None,
-        having=None,
-        order_by=None,
-        sql=None,
-    ):
-        self._ops = operator
-        self._from_ = from_
-        self._select = select
-        self._join = join
-        self._where = where
-        self._group_by = group_by
-        self._having = having
-        self._order_by = order_by
-        self._sql = sql
-
-    def __copy__(self):
-        return type(self)(
-            self._ops,
-            self._from_,
-            self._select,
-            self._join,
-            self._where,
-            self._group_by,
-            self._having,
-            self._order_by,
-            self._sql,
-        )
-
-    def __str__(self):
-        self._make_qry()
-        return self._qry
-
-    def _args2str(self, args, sep):
-        """
-        Parse a tuple of str, or iterator of str,
-        into a combined str, fit to be used as part of query.
-
-        Parameters
-        ----------
-        args : (str,) or ([str],)
-            Either a tuple of elemental and/or combined str
-            , or a tuple with first and only element
-            being a iterator of elemental str.
-        sep : str
-            Seperator used to seperate elemental str.
-
-        Returns
-        -------
-        str
-            The combined str.
-
-        Examples
-        --------
-        >>> import dwopt
-        >>> dwopt._qry._Qry._args2str(_,('a,b,c',),',')
-            'a,b,c'
-        >>> dwopt._qry._Qry._args2str(_,('a','b','c',),',')
-            'a,b,c'
-        >>> dwopt._qry._Qry._args2str(_,(['a','b','c'],),',')
-            'a,b,c'
-        >>> dwopt._qry._Qry._args2str(_,(('a','b','c'),),',')
-            'a,b,c'
-        """
-        L = len(args)
-        if L == 0:
-            res = None
-        elif L == 1:
-            arg = args[0]
-            if isinstance(arg, str):
-                res = arg
-            else:
-                res = sep.join(arg)
-        else:
-            res = sep.join(args)
-        return res
-
-    def _make_cls(self, key, load, na=""):
-        """Add keyword to clause payload"""
-        return f"{key}{load}" if load is not None else na
-
-    def _make_qry(self):
-        """Combine query components."""
-        if self._sql is not None:
-            self._qry = self._sql
-        else:
-            select = self._make_cls("select ", self._select, "select *")
-            from_ = self._make_cls("from ", self._from_, "from test")
-            join = self._make_cls("\n", self._join)
-            where = self._make_cls("\nwhere ", self._where)
-            group_by = self._make_cls("\ngroup by ", self._group_by)
-            having = self._make_cls("\nhaving ", self._having)
-            order_by = self._make_cls("\norder by ", self._order_by)
-            self._qry = (
-                select
-                + (" " if select == "select *" else "\n")
-                + from_
-                + join
-                + where
-                + group_by
-                + having
-                + order_by
-            )
-            if self._ops._dialect == "oc":
-                self._qry = self._qry.replace("select", "select /*+PARALLEL (4)*/")
-
-    def bin(self, out=None):
-        """WIP"""
-        raise NotImplementedError
-
-    def case(self, col, *args, cond=None, els="NULL"):
-        """Add a case when clause to the select clause.
-
-        Calling this method multiple times would add multiple statements.
-
-        Parameters
-        ----------
-        col : str
-            Column name of the resulting column.
-        *args : str
-            Positional argument in form 'condition then treatement'.
-        cond : dict
-            Dictionary of condition str to treatment str mappings.
-        els : str
-            Value for else clause, default ``NULL``.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> q = lt.qry('iris').case('mt4',"petal_length > 4 then 1", els=0)
-        >>> q.print()
-        select *
-            ,case when petal_length > 4 then 1 else 0 end as mt4
-        from iris
-        >>> q.valc('species','avg(mt4) pct_mt4')
-           species   n  pct_mt4
-        0  sicolor  50     0.68
-        1   setosa  50     0.00
-        2  rginica  50     1.00
-
-        Combine case when, value counts, and pivot:
-
-        >>> from dwopt import lt as d
-        >>> d.iris(q=1).case('cat', # doctest: +SKIP
-        ...     "petal_length > 5             then '5+'",
-        ...     "petal_length between 2 and 5 then '2-5'",
-        ...     "petal_length < 2             then '-2'",
-        ... ).valc('species, cat').pivot('species','cat','n')
-        cat        -2   2-5    5+
-        species
-        rginica   NaN   9.0  41.0
-        setosa   50.0   NaN   NaN
-        sicolor   NaN  49.0   1.0
-
-        Use the ``cond`` argument:
-
-        >>> from dwopt import pg
-        >>> pg.mtcars()
-        >>> pg.qry("mtcars").select('name, mpg').case('cat', cond = {
-        ...         'mpg between 10 and 20':15,
-        ...         'mpg between 20 and 30':25,
-        ...         'mpg between 30 and 40':35,
-        ...     }
-        ... ).print()
-        select name, mpg
-            ,case
-                when mpg between 10 and 20 then 15
-                when mpg between 20 and 30 then 25
-                when mpg between 30 and 40 then 35
-                else NULL
-            end as cat
-        from mtcars
-        """
-        _ = self.__copy__()
-        if cond is not None:
-            for i, j in cond.items():
-                args = args + (f"{i} then {j}",)
-        if len(args) == 0:
-            raise TypeError(
-                "qry.case() takes at least one args or cond argument (0 given)"
-            )
-        elif len(args) == 1 and len(args[0]) < 35:
-            cls = f"\n    ,case when {args[0]} else {els} end as {col}"
-        else:
-            cls = self._args2str(args, "\n        when ")
-            cls = (
-                "\n    ,case"
-                f"\n        when {cls}"
-                f"\n        else {els}"
-                f"\n    end as {col}"
-            )
-        if _._select is None:
-            _._select = "*" + cls
-        else:
-            _._select = _._select + cls
-        return _
-
-    def cols(self, out=None):
-        """Fetch column names of the sub query table.
-
-        Args
-        --------
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        Column names as list of str. Or full query as str.
-
-        Examples
-        --------
-        >>> from dwopt import lt as d
-        >>> d.iris()
-        >>> d.qry('iris').cols()
-        ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species']
-        >>> d.qry('iris').cols(out=1)
-        with x as (
-            select * from iris
-        )
-        select * from x where 1=2
-
-        Use with comprehension to obtain subsets:
-
-        >>> from dwopt import pg as d
-        >>> d.create_schema('test')
-        >>> q = d.iris('test.iris', q=1)
-        >>> [i for i in q.cols() if i != 'species']
-        ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
-        """
-        q = "select * from x where 1=2"
-        if out is None:
-            return self.run(q).columns.tolist()
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def dist(self, *args, out=None):
-        """Count number of distinct occurances of data.
-
-        Works on specified columns, or combination of columns, of the sub query table.
-
-        Args
-        ----------
-        *args : str or [str]
-            Either column names as str, or iterator of column name str.
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        pandas.Series
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> q = lt.mtcars(q=1)
-        >>> q.dist('mpg')
-        count(distinct mpg)    25
-        Name: 0, dtype: int64
-        >>> q.dist('mpg', 'cyl')
-        count(distinct mpg)    25
-        count(distinct cyl)     3
-        Name: 0, dtype: int64
-        >>> q.dist(['mpg', 'cyl'])
-        count(distinct mpg || '_' || cyl)    27
-        Name: 0, dtype: int64
-        >>> q.dist(*q.cols()[:4])
-        count(distinct name)    32
-        count(distinct mpg)     25
-        count(distinct cyl)      3
-        count(distinct disp)    27
-        Name: 0, dtype: int64
-
-        >>> from dwopt import pg
-        >>> pg.create_schema('test')
-        >>> q = pg.mtcars('test.mtcars', q=1)
-        >>> q.dist('mpg', ['mpg', 'cyl'], out=1) # doctest: +SKIP
-        with x as (
-            select * from test.mtcars
-        )
-        select
-            count(distinct mpg)
-            ,count(distinct mpg || '_' || cyl)
-        from x
-        >>> q.dist('mpg', ['mpg', 'cyl'])
-        count    25
-        count    27
-        Name: 0, dtype: int64
-        """
-        _ = (" || '_' || ".join(_) if not isinstance(_, str) else _ for _ in args)
-        _ = "".join(
-            f"    ,count(distinct {j})\n" if i else f"    count(distinct {j})\n"
-            for i, j in enumerate(_)
-        )
-        q = "select \n" f"{_}" "from x"
-
-        if out is None:
-            return self.run(q).iloc[0, :]
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def five(self, out=None):
-        """WIP"""
-        raise NotImplementedError
-
-    def from_(self, from_):
-        """Add the from clause to query.
-
-        Alternative to simply specifying table
-        name as the only argument of the qry method. Use the qry method.
-
-        Parameters
-        ----------
-        from_ : str
-            Table name str.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry().from_("iris").print()
-        select * from iris
-        """
-        _ = self.__copy__()
-        _._from_ = from_
-        return _
-
-    def group_by(self, *args):
-        """Add the group by clause to query.
-
-        Parameters
-        ----------
-        *args : str or [str]
-            Group by columns in str format, or iterator of them.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> (
-        ...     lt.qry('mtcars')
-        ...     .select('hp, count(1) n, avg(mpg)')
-        ...     .group_by('hp')
-        ...     .having("avg(mpg) > 30")
-        ...     .run()
-        ... )
-            hp  n  avg(mpg)
-        0   52  1      30.4
-        1   65  1      33.9
-        2  113  1      30.4
-        >>> (
-        ...     lt.qry('mtcars')
-        ...     .select('hp, cyl, count(1) n, avg(mpg)')
-        ...     .group_by('hp,cyl')
-        ...     #.group_by('hp', 'cyl') #same effect
-        ...     #.group_by(['hp', 'cyl']) #same effect
-        ...     .having("avg(mpg) > 30")
-        ...     .print()
-        ... )
-        select hp, cyl, count(1) n, avg(mpg)
-        from mtcars
-        group by hp,cyl
-        having avg(mpg) > 30
-        """
-        _ = self.__copy__()
-        _._group_by = self._args2str(args, ",")
-        return _
-
-    def hash(self, *args, out=None):
-        """Calculate a simple oracle hash for table.
-
-        Arrive at a indicative hash value for a number of columns or all columns of
-        a sub query table.
-        Hash value is a number or symbol that is calculated from data
-        , and is sensitive to any small changes in data. It serves as method to
-        detect if any data element in data is changed.
-
-        Args
-        ----------
-        *args : str or [str]
-            Column names in str. If no value is given, a cols method will be
-            performed to fetch the list of all columns, from which a hash will be
-            calculated.
-            Also allow passing in a single list of str column names.
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        int
-
-        Examples
-        --------
-        ::
-
-            from dwopt import oc
-            q = oc.iris(q=1)
-            q.hash('petal_length')
-            q.hash('petal_length', 'petal_width')
-            q.hash(['petal_length', 'petal_width'])
-            q.hash(out=1)
-        """
-        if self._ops._dialect != "oc":
-            raise NotImplementedError
-        if len(args) == 0:
-            args = self.cols()
-        _ = args[0] if len(args) == 1 and not isinstance(args[0], str) else args
-        _ = " || '_' || ".join(_)
-        q = (
-            "select/*+ PARALLEL(4) */ \n"
-            "    ora_hash(sum(ora_hash(\n"
-            f"        {_}\n"
-            "    ) - 4294967296/2)) hash\n"
-            "from x"
-        )
-        if out is None:
-            return self.run(q).iloc[0, 0]
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def having(self, *args):
-        """Add the having clause to query.
-
-        Parameters
-        ----------
-        *args : str or [str]
-            Conditions in str format, or iterator of them.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> q = (
-        ...     lt.qry('mtcars')
-        ...     .select('hp, count(1) n, avg(mpg)')
-        ...     .group_by('hp')
-        ...     .having("count(1) > 1", "avg(mpg) > 15")
-        ...     .order_by('n desc')
-        ... )
-        >>>
-        >>> q.print()
-        select hp, count(1) n, avg(mpg)
-        from mtcars
-        group by hp
-        having count(1) > 1
-            and avg(mpg) > 15
-        order by n desc
-        >>> q.run()
-            hp  n   avg(mpg)
-        0  180  3  16.300000
-        1  175  3  19.200000
-        2  110  3  21.133333
-        3  150  2  15.350000
-        4  123  2  18.500000
-        5   66  2  29.850000
-        """
-        _ = self.__copy__()
-        _._having = self._args2str(args, "\n    and ")
-        return _
-
-    def head(self, out=None):
-        """Fetch top 5 rows of the sub query table.
-
-        Args
-        -------
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry("iris").head()
-           sepal_length  sepal_width  petal_length  petal_width species
-        0           5.1          3.5           1.4          0.2  setosa
-        1           4.9          3.0           1.4          0.2  setosa
-        2           4.7          3.2           1.3          0.2  setosa
-        3           4.6          3.1           1.5          0.2  setosa
-        4           5.0          3.6           1.4          0.2  setosa
-        """
-        if self._ops._dialect == "oc":
-            q = "select * from x where rownum <= 5"
-        else:
-            q = "select * from x limit 5"
-        if out is None:
-            return self.run(q)
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def join(self, sch_tbl_nme, *args, how="left"):
-        """Add a join clause to query.
-
-        Calling this method multiple times would add multiple clauses.
-
-        Parameters
-        ----------
-        sch_tbl_nme : str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-        *args : str
-            Joining conditions in str format.
-        how : str
-            The join keyword in str format, for example: ``inner``, ``cross``.
-            Default ``left``.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> q = (
-        ...     lt.qry('mtcars a').select('a.cyl, b.mpg')
-        ...     .join('mtcars b','a.name = b.name')
-        ... )
-        >>> q.valc('cyl', 'avg(mpg)')
-           cyl   n   avg(mpg)
-        0    8  14  15.100000
-        1    4  11  26.663636
-        2    6   7  19.742857
-        >>> q.valc('cyl', 'avg(mpg)', out=1) # doctest: +SKIP
-        with x as (
-            select a.cyl, b.mpg
-            from mtcars a
-            left join mtcars b
-                on a.name = b.name
-        )
-        select
-            cyl
-            ,count(1) n
-            ,avg(mpg)
-        from x
-        group by cyl
-        order by n desc
-
-        >>> (
-        ...     lt.qry('mtcars a').select('a.cyl, b.mpg, c.hp')
-        ...     .join('mtcars b','a.name = b.name')
-        ...     .join('mtcars c','a.name = c.name')
-        ...     .valc('cyl', 'avg(mpg), avg(hp)')
-        ... )
-           cyl   n   avg(mpg)     avg(hp)
-        0    8  14  15.100000  209.214286
-        1    4  11  26.663636   82.636364
-        2    6   7  19.742857  122.285714
-
-        Inject a sub-query into the ``sch_tbl_nme`` argument:
-
-        >>> sql = "select cyl from mtcars group by cyl having count(1) > 10"
-        >>> q = (
-        ...     lt.qry('mtcars a').select('a.cyl, a.mpg')
-        ...     .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
-        ... )
-        >>> q.valc('cyl', 'avg(mpg)')
-           cyl   n   avg(mpg)
-        0    8  14  15.100000
-        1    4  11  26.663636
-        >>> q.valc('cyl', 'avg(mpg)', out=1) # doctest: +SKIP
-        with x as (
-            select a.cyl, a.mpg
-            from mtcars a
-            inner join (select cyl from mtcars group by cyl having count(1) > 10) b
-                on a.cyl = b.cyl
-        )
-        select
-            cyl
-            ,count(1) n
-            ,avg(mpg)
-        from x
-        group by cyl
-        order by n desc
-        """
-        _ = self.__copy__()
-        on = self._args2str(args, "\n    and ")
-        cls = f"{how} join {sch_tbl_nme}" f"\n    on {on}"
-        if _._join is not None:
-            _._join = _._join + "\n" + cls
-        else:
-            _._join = cls
-        return _
-
-    def len(self, out=None):
-        """Length of the sub query table.
-
-        Args
-        -------
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        int
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').len()
-        150
-        >>> lt.mtcars(q=1).len()
-        32
-        """
-        q = "select count(1) from x"
-        if out is None:
-            return self.run(q).iloc[0, 0]
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def mimx(self, col, out=None):
-        """Fetch maximum and minimum values of a column.
-
-        Args
-        ----------
-        col : str
-            Column name as str.
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        pandas.Series
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').mimx('sepal_width')
-        max(sepal_width)    4.4
-        min(sepal_width)    2.0
-        Name: 0, dtype: float64
-        """
-        q = "select \n" f"    max({col}),min({col})\n" "from x"
-        if out is None:
-            return self.run(q).iloc[0, :]
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def order_by(self, *args):
-        """
-        Add the order by clause to query.
-
-        Parameters
-        ----------
-        *args : str or [str]
-            Order by names in str format, or iterator of them.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> q = (
-        ...     lt.qry('mtcars')
-        ...     .select('hp, count(1) n, avg(mpg)')
-        ...     .group_by('hp')
-        ...     .having("count(1) > 1", "avg(mpg) > 15")
-        ...     .order_by('n desc')
-        ... )
-        >>>
-        >>> q.run()
-            hp  n   avg(mpg)
-        0  180  3  16.300000
-        1  175  3  19.200000
-        2  110  3  21.133333
-        3  150  2  15.350000
-        4  123  2  18.500000
-        5   66  2  29.850000
-        """
-        _ = self.__copy__()
-        _._order_by = self._args2str(args, ",")
-        return _
-
-    def pct(self):
-        """WIP"""
-        raise NotImplementedError
-
-    def piv(self):
-        """WIP"""
-        raise NotImplementedError
-
-    def print(self, sum_qry=None):
-        """Print the built query.
-
-        * If the ``sum_qry`` argument is not given value,
-          print underlying query as it is.
-        * If a value is given, enclose the underlying query into a with
-          clause, attach the summary query after it, print the full query.
-
-        See also
-        ---------
-        :meth:`dwopt._qry._Qry.str`
-        :meth:`dwopt._qry._Qry.run`
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').select('count(1)').print()
-        select count(1)
-        from iris
-        >>> lt.qry('iris').print('select count(1) from x')
-        with x as (
-            select * from iris
-        )
-        select count(1) from x
-        """
-        print(self.str(sum_qry))
-
-    def run(self, sum_qry=None, **kwargs):
-        """Run the built query.
-
-        * If the ``sum_qry`` argument is not given value,
-          run underlying query as it is.
-        * If a value is given, enclose the underlying query into a with
-          clause, attach the summary query after it, run the full query.
-
-        Args
-        ----------
-        sum_qry: str
-            Summary query string.
-        **kwargs:
-            Keyword arguments to pass on to database operator's run method.
-
-        Returns
-        -------
-        pandas.DataFrame or None
-            Returned by the database operator's
-            :meth:`dwopt.dbo._Db.run` method.
-
-        See also
-        ---------
-        :meth:`dwopt._qry._Qry.str`
-        :meth:`dwopt._qry._Qry.print`
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').select('count(1)').run()
-           count(1)
-        0       150
-        >>> lt.qry('iris').run('select count(1) from x')
-           count(1)
-        0       150
-        >>> lt.qry('iris').where('petal_length>:x').run(
-        ...     'select count(1) from x', mods={'x':2}
-        ... )
-           count(1)
-        0       100
-        """
-        qry = self.str(sum_qry)
-        return self._ops.run(qry, **kwargs)
-
-    def select(self, *args, sep=","):
-        """
-        Add the select clause to query.
-
-        Parameters
-        ----------
-        *args : str or [str]
-            Column name str as positional arguments
-            , or an iterator of str column names.
-        sep : str
-            Symbol used for seperating column names, default ``,``.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> q = lt.iris(q=1)
-        >>> q.select("species, sepal_length").print()
-        select species, sepal_length
-        from iris
-        >>> q.select("species", "sepal_length").print()
-        select species,sepal_length
-        from iris
-        >>> q.select(["species", "sepal_length"]).print()
-        select species,sepal_length
-        from iris
-        >>> q.select(["species", "sepal_length + 2 as sepal_length_new"]).print()
-        select species,sepal_length + 2 as sepal_length_new
-        from iris
-        """
-        _ = self.__copy__()
-        _._select = self._args2str(args, sep)
-        return _
-
-    def sql(self, sql):
-        """Replace the underlying query by specified sql.
-
-        This allows arbituary advanced sql to be incorporated into framework.
-
-        Parameters
-        ----------
-        sql : str
-            Sql code in str format.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> q = lt.qry().sql("select * from iris where sepal_length > 7")
-        >>> q.len()
-        12
-        >>> q.print()
-        select * from iris where sepal_length > 7
-        """
-        _ = self.__copy__()
-        _._sql = sql
-        return _
-
-    def str(self, sum_qry=None):
-        """Return the built query as str.
-
-        * If the ``sum_qry`` argument is not given value,
-          return underlying query as it is.
-        * If a value is given, enclose the underlying query into a with
-          clause, attach the summary query after it, return the full query.
-
-        Args
-        ----------
-        sum_qry: str
-            Summary query string.
-
-        Returns
-        ---------
-        str
-
-        See also
-        ---------
-        :meth:`dwopt._qry._Qry.print`
-        :meth:`dwopt._qry._Qry.run`
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').select('count(1)').str()
-        'select count(1)\\nfrom iris'
-        >>> lt.qry('iris').str('select count(1) from x')
-        'with x as (\\n    select * from iris\\n)\\nselect count(1) from x'
-        """
-        self._make_qry()
-        if sum_qry is not None:
-            _ = self._qry.replace("\n", "\n    ")
-            _ = "with x as (\n" f"    {_}\n" ")"
-            qry = f"{_}\n{sum_qry}"
-        else:
-            qry = self._qry
-        return qry
-
-    def top(self, out=None):
-        """Fetch top row of the sub query table.
-
-        Args
-        -------
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        pandas.Series
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> lt.qry('mtcars').top()
-        name    Mazda RX4
-        mpg          21.0
-        cyl             6
-        disp        160.0
-        hp            110
-        drat          3.9
-        wt           2.62
-        qsec        16.46
-        vs              0
-        am              1
-        gear            4
-        carb            4
-        Name: 0, dtype: object
-
-        Use ``print`` and ``to_string`` to force display of all columns:
-
-        >>> print(lt.iris(q=1).top().to_string())
-        sepal_length       5.1
-        sepal_width        3.5
-        petal_length       1.4
-        petal_width        0.2
-        species         setosa
-        """
-        if self._ops._dialect == "oc":
-            q = "select * from x where rownum<=1"
-        else:
-            q = "select * from x limit 1"
-        if out is None:
-            res = self.run(q)
-            if res.empty:
-                return pd.Series(index=res.columns)
-            else:
-                return res.iloc[
-                    0,
-                ]
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def valc(self, group_by, agg=None, order_by=None, n=True, out=None):
-        """Value count of a column or combination of columns.
-
-        A value count is a
-        group by query, with total number of row of each group calculated.
-        Also allow custom summary calculation, and custom order by clauses
-        to be added.
-
-        Args
-        ----------
-        group_by : str
-            Group by clause as str.
-        agg : str
-            Custom aggeregation clause as str.
-        order_by : str
-            Order by clause as str.
-        n : Bool
-            Should the value count column be automatically created or not. Default
-            to be True.
-        out: int
-            Output mode. None to run full query, 1 to print full query,
-            2 to return full query as str. Default None.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Examples
-        --------
-        Various configuration of value counts:
-
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.qry('iris').valc('species', 'avg(petal_length)')
-           species   n  avg(petal_length)
-        0  sicolor  50              4.260
-        1   setosa  50              1.462
-        2  rginica  50              5.552
-        >>> lt.qry('iris').valc('species', 'avg(petal_length) avg', 'avg desc')
-           species   n    avg
-        0  rginica  50  5.552
-        1  sicolor  50  4.260
-        2   setosa  50  1.462
-        >>> lt.qry('iris').valc('species', 'avg(petal_length)', n=False)
-           species  avg(petal_length)
-        0  rginica              5.552
-        1   setosa              1.462
-        2  sicolor              4.260
-        >>> lt.qry('iris').valc('species', 'avg(petal_length)', out=1)# doctest: +SKIP
-        with x as (
-            select * from iris
-        )
-        select
-            species
-            ,count(1) n
-            ,avg(petal_length)
-        from x
-        group by species
-        order by n desc
-
-        Excel-pivot-table-like API:
-
-        .. code-block :: python
-
-            from dwopt import lt, make_test_tbl
-            import logging
-            logging.basicConfig(level = logging.INFO)
-            _ = make_test_tbl(lt)
-            (
-                lt.qry('test').where('score>0.5', 'dte is not null', 'cat is not null')
-                .valc('dte, cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
-                .pivot('dte', 'cat')
-            )
-
-        Logs showing sql used:
-
-        .. code-block :: sql
-
-            INFO:dwopt.dbo:running:
-            with x as (
-                select * from test
-                where score>0.5
-                    and dte is not null
-                    and cat is not null
-            )
-            select
-                dte, cat
-                ,count(1) n
-                ,avg(score) avgscore, round(sum(amt)/1e3,2) total
-            from x
-            group by dte, cat
-            order by n desc
-            INFO:dwopt.dbo:done
-
-        Results::
-
-                           n        avgscore             total
-            cat         test train      test     train    test   train
-            dte
-            2022-01-01  1140  1051  2.736275  2.800106  565.67  530.09
-            2022-02-02  1077  1100  2.759061  2.748898  536.68  544.10
-            2022-03-03  1037  1072  2.728527  2.743825  521.54  528.85
-
-        Combine case when, value counts, and pivot:
-
-        >>> from dwopt import lt as d
-        >>> d.iris(q=1).case('cat', # doctest: +SKIP
-        ...     "petal_length > 5             then '5+'",
-        ...     "petal_length between 2 and 5 then '2-5'",
-        ...     "petal_length < 2             then '-2'",
-        ... ).valc('species, cat').pivot('species','cat','n')
-        cat        -2   2-5    5+
-        species
-        rginica   NaN   9.0  41.0
-        setosa   50.0   NaN   NaN
-        sicolor   NaN  49.0   1.0
-
-        Make summary for all relevant columns via generated statements:
-
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> q = lt.qry('iris')
-        >>> agg = ', '.join(f'avg({col}) {col}' for col in q.cols() if col != 'species')
-        >>> q.valc('species', agg)
-           species   n  sepal_length  sepal_width  petal_length  petal_width
-        0  sicolor  50         5.936        2.770         4.260        1.326
-        1   setosa  50         5.006        3.428         1.462        0.246
-        2  rginica  50         6.588        2.974         5.552        2.026
-        """
-        group_by_cls = ",".join(group_by) if not isinstance(group_by, str) else group_by
-        if agg is None:
-            agg_cls = ""
-        elif isinstance(agg, str):
-            agg_cls = f"    ,{agg}\n"
-        else:
-            agg_cls = "".join(f"    ,{_}\n" for _ in agg)
-        if order_by is None:
-            if n:
-                order_by_cls = "n desc"
-            else:
-                order_by_cls = group_by_cls
-        else:
-            order_by_cls = order_by
-        q = (
-            "select \n"
-            f"    {group_by_cls}\n"
-            f"{f'    ,count(1) n{chr(10)}' if n else ''}"
-            f"{agg_cls}"
-            "from x\n"
-            f"group by {group_by_cls}\n"
-            f"order by {order_by_cls}"
-        )
-        if out is None:
-            return self.run(q)
-        elif out == 1:
-            self.print(q)
-        elif out == 2:
-            return self.str(q)
-        else:
-            raise ValueError("Invalid out, one of: None, 1, 2")
-
-    def where(self, *args):
-        """
-        Add the where clause to query.
-
-        Parameters
-        ----------
-        *args : str or [str]
-            Conditions in str format, or iterator of condition str.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-            New query object with clause added.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> lt.qry('mtcars').where("cyl = 4").len()
-        11
-        >>> lt.qry('mtcars').where("cyl = 4", "vs = 0").run()
-                    name   mpg  cyl   disp  hp  drat    wt  qsec  vs  am  gear  carb
-        0  Porsche 914-2  26.0    4  120.3  91  4.43  2.14  16.7   0   1     5     2
-        >>> lt.qry('mtcars').where("cyl = 4 and vs = 0").print()
-        select * from mtcars
-        where cyl = 4 and vs = 0
-        """
-        _ = self.__copy__()
-        _._where = self._args2str(args, "\n    and ")
-        return _
+import pandas as pd
+
+
+class _Qry:
+    """
+    The query class.
+
+    See examples for quick-start.
+
+    Automatically instantiated via the :meth:`~dwopt.dbo._Db.qry` method from the
+    :class:`database operator <dwopt.dbo._Db>` objects.
+
+    It is possible to pass in all needed parameters when calling the method.
+    But it is clearer to only pass in one positional argument as table name,
+    and use the :ref:`clause methods` to build up a query instead.
+
+    Parameters
+    ----------
+    operator : dwopt.db._Db
+        Database operator object to operate on generated queries.
+    from_ : str
+        Query table name.
+    select: str
+        Columns.
+    join : str
+        Join clause.
+    where : str
+        Conditions.
+    group_by : str
+        Group by names.
+    having : str
+        Conditions.
+    order_by : str
+        Order by names.
+    sql : str
+        Sql code.
+
+    Notes
+    -----
+    .. _The summary query building framework:
+
+    **The summary query building framework**
+
+    Queries are flexibly built as a combination of a ``sub query``
+    and a ``summary query`` from templates.
+    Point of ``sub query`` is to be a flexible complementary pre-processing step,
+    productivity gain comes from the ``summary query`` templates.
+
+    Example:
+
+    .. code-block:: sql
+
+        -- Sub query: arbituary query within a with clause named x
+        with x as (
+            select * from test
+            where score>0.5
+                and dte is not null
+                and cat is not null
+        )
+        -- Summary query: generated from templates
+        select
+            dte, cat
+            ,count(1) n
+            ,avg(score) avgscore, round(sum(amt)/1e3,2) total
+        from x
+        group by dte, cat
+        order by n desc
+
+    Corresponding code::
+
+        from dwopt import lt, make_test_tbl
+        _ = make_test_tbl(lt)
+        (
+            lt.qry('test').where('score>0.5', 'dte is not null', 'cat is not null')
+            .valc(
+                'dte, cat',
+                'avg(score) avgscore, round(sum(amt)/1e3,2) total',
+                out=1
+            )
+        )
+
+    Use the :ref:`clause methods` to iteratively
+    piece together a query, or use the :meth:`~dwopt._qry._Qry.sql` method to provide
+    an arbituary query. This created query will then be placed inside a
+    with block and become the ``sub query`` on invocation of any summary methods.
+
+    The ``summary query`` is built from parameterized templates via
+    the :ref:`summary methods`. Calling one of them completes the whole query
+    and immediately runs it.
+
+    This way for large tables, heavy intermediate results from the ``sub query``
+    are never realized outside of the database engine,
+    while light summary results are placed in python for analysis.
+
+    Examples
+    --------
+
+    Create and use qry object using the :meth:`~dwopt.dbo._Db.qry` method from the
+    :class:`database operator <dwopt.dbo._Db>` objects:
+
+    >>> from dwopt import lt
+    >>> lt.iris()
+    >>> lt.qry('iris').len()
+    150
+    >>> lt.qry('iris').valc('species', 'avg(petal_length)')
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+    >>> lt.qry('iris').where('petal_length > 2').valc('species', out=1)# doctest: +SKIP
+    with x as (
+        select * from iris
+        where petal_length > 2
+    )
+    select
+        species
+        ,count(1) n
+    from x
+    group by species
+    order by n desc
+
+    Iteratively piece together a query using the :ref:`clause methods`:
+
+    >>> from dwopt import lt
+    >>> lt.mtcars()
+    >>> sql = "select cyl from mtcars group by cyl having count(1) > 10"
+    >>> q = (
+    ...     lt.qry('mtcars a')
+    ...     .select('a.cyl, count(1) n, avg(a.mpg)')
+    ...     .case('cat', "a.cyl = 8 then 1", els=0)
+    ...     .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
+    ...     .group_by('a.cyl')
+    ...     .having('count(1) > 10')
+    ...     .order_by('n desc')
+    ... )
+    >>>
+    >>> q.print()
+    select a.cyl, count(1) n, avg(a.mpg)
+        ,case when a.cyl = 8 then 1 else 0 end as cat
+    from mtcars a
+    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
+        on a.cyl = b.cyl
+    group by a.cyl
+    having count(1) > 10
+    order by n desc
+    >>> q.run()
+       cyl   n  avg(a.mpg)  cat
+    0    8  14   15.100000    1
+    1    4  11   26.663636    0
+
+    Use the :ref:`summary methods` for analysis:
+
+    >>> from dwopt import pg as d
+    >>> d.iris('iris')
+    >>> q = d.qry('iris').where('petal_length > 2')
+    >>> q.top()
+    sepal_length        7.0
+    sepal_width         3.2
+    petal_length        4.7
+    petal_width         1.4
+    species         sicolor
+    Name: 0, dtype: object
+    >>> q.head()
+       sepal_length  sepal_width  petal_length  petal_width  species
+    0           7.0          3.2           4.7          1.4  sicolor
+    1           6.4          3.2           4.5          1.5  sicolor
+    2           6.9          3.1           4.9          1.5  sicolor
+    3           5.5          2.3           4.0          1.3  sicolor
+    4           6.5          2.8           4.6          1.5  sicolor
+    >>> q.len()
+    100
+    >>> agg = ', '.join(f'avg({col}) {col}' for col in q.cols() if col != 'species')
+    >>> q.valc('species', agg)
+       species   n  sepal_length  sepal_width  petal_length  petal_width
+    0  sicolor  50         5.936        2.770         4.260        1.326
+    1  rginica  50         6.588        2.974         5.552        2.026
+    """
+
+    def __init__(
+        self,
+        operator,
+        from_=None,
+        select=None,
+        join=None,
+        where=None,
+        group_by=None,
+        having=None,
+        order_by=None,
+        sql=None,
+    ):
+        self._ops = operator
+        self._from_ = from_
+        self._select = select
+        self._join = join
+        self._where = where
+        self._group_by = group_by
+        self._having = having
+        self._order_by = order_by
+        self._sql = sql
+
+    def __copy__(self):
+        return type(self)(
+            self._ops,
+            self._from_,
+            self._select,
+            self._join,
+            self._where,
+            self._group_by,
+            self._having,
+            self._order_by,
+            self._sql,
+        )
+
+    def __str__(self):
+        self._make_qry()
+        return self._qry
+
+    def _args2str(self, args, sep):
+        """
+        Parse a tuple of str, or iterator of str,
+        into a combined str, fit to be used as part of query.
+
+        Parameters
+        ----------
+        args : (str,) or ([str],)
+            Either a tuple of elemental and/or combined str
+            , or a tuple with first and only element
+            being a iterator of elemental str.
+        sep : str
+            Seperator used to seperate elemental str.
+
+        Returns
+        -------
+        str
+            The combined str.
+
+        Examples
+        --------
+        >>> import dwopt
+        >>> dwopt._qry._Qry._args2str(_,('a,b,c',),',')
+            'a,b,c'
+        >>> dwopt._qry._Qry._args2str(_,('a','b','c',),',')
+            'a,b,c'
+        >>> dwopt._qry._Qry._args2str(_,(['a','b','c'],),',')
+            'a,b,c'
+        >>> dwopt._qry._Qry._args2str(_,(('a','b','c'),),',')
+            'a,b,c'
+        """
+        L = len(args)
+        if L == 0:
+            res = None
+        elif L == 1:
+            arg = args[0]
+            if isinstance(arg, str):
+                res = arg
+            else:
+                res = sep.join(arg)
+        else:
+            res = sep.join(args)
+        return res
+
+    def _make_cls(self, key, load, na=""):
+        """Add keyword to clause payload"""
+        return f"{key}{load}" if load is not None else na
+
+    def _make_qry(self):
+        """Combine query components."""
+        if self._sql is not None:
+            self._qry = self._sql
+        else:
+            select = self._make_cls("select ", self._select, "select *")
+            from_ = self._make_cls("from ", self._from_, "from test")
+            join = self._make_cls("\n", self._join)
+            where = self._make_cls("\nwhere ", self._where)
+            group_by = self._make_cls("\ngroup by ", self._group_by)
+            having = self._make_cls("\nhaving ", self._having)
+            order_by = self._make_cls("\norder by ", self._order_by)
+            self._qry = (
+                select
+                + (" " if select == "select *" else "\n")
+                + from_
+                + join
+                + where
+                + group_by
+                + having
+                + order_by
+            )
+            if self._ops._dialect == "oc":
+                self._qry = self._qry.replace("select", "select /*+PARALLEL (4)*/")
+
+    def bin(self, out=None):
+        """WIP"""
+        raise NotImplementedError
+
+    def case(self, col, *args, cond=None, els="NULL"):
+        """Add a case when clause to the select clause.
+
+        Calling this method multiple times would add multiple statements.
+
+        Parameters
+        ----------
+        col : str
+            Column name of the resulting column.
+        *args : str
+            Positional argument in form 'condition then treatement'.
+        cond : dict
+            Dictionary of condition str to treatment str mappings.
+        els : str
+            Value for else clause, default ``NULL``.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> q = lt.qry('iris').case('mt4',"petal_length > 4 then 1", els=0)
+        >>> q.print()
+        select *
+            ,case when petal_length > 4 then 1 else 0 end as mt4
+        from iris
+        >>> q.valc('species','avg(mt4) pct_mt4')
+           species   n  pct_mt4
+        0  sicolor  50     0.68
+        1   setosa  50     0.00
+        2  rginica  50     1.00
+
+        Combine case when, value counts, and pivot:
+
+        >>> from dwopt import lt as d
+        >>> d.iris(q=1).case('cat', # doctest: +SKIP
+        ...     "petal_length > 5             then '5+'",
+        ...     "petal_length between 2 and 5 then '2-5'",
+        ...     "petal_length < 2             then '-2'",
+        ... ).valc('species, cat').pivot('species','cat','n')
+        cat        -2   2-5    5+
+        species
+        rginica   NaN   9.0  41.0
+        setosa   50.0   NaN   NaN
+        sicolor   NaN  49.0   1.0
+
+        Use the ``cond`` argument:
+
+        >>> from dwopt import pg
+        >>> pg.mtcars()
+        >>> pg.qry("mtcars").select('name, mpg').case('cat', cond = {
+        ...         'mpg between 10 and 20':15,
+        ...         'mpg between 20 and 30':25,
+        ...         'mpg between 30 and 40':35,
+        ...     }
+        ... ).print()
+        select name, mpg
+            ,case
+                when mpg between 10 and 20 then 15
+                when mpg between 20 and 30 then 25
+                when mpg between 30 and 40 then 35
+                else NULL
+            end as cat
+        from mtcars
+        """
+        _ = self.__copy__()
+        if cond is not None:
+            for i, j in cond.items():
+                args = args + (f"{i} then {j}",)
+        if len(args) == 0:
+            raise TypeError(
+                "qry.case() takes at least one args or cond argument (0 given)"
+            )
+        elif len(args) == 1 and len(args[0]) < 35:
+            cls = f"\n    ,case when {args[0]} else {els} end as {col}"
+        else:
+            cls = self._args2str(args, "\n        when ")
+            cls = (
+                "\n    ,case"
+                f"\n        when {cls}"
+                f"\n        else {els}"
+                f"\n    end as {col}"
+            )
+        if _._select is None:
+            _._select = "*" + cls
+        else:
+            _._select = _._select + cls
+        return _
+
+    def cols(self, out=None):
+        """Fetch column names of the sub query table.
+
+        Args
+        --------
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        Column names as list of str. Or full query as str.
+
+        Examples
+        --------
+        >>> from dwopt import lt as d
+        >>> d.iris()
+        >>> d.qry('iris').cols()
+        ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species']
+        >>> d.qry('iris').cols(out=1)
+        with x as (
+            select * from iris
+        )
+        select * from x where 1=2
+
+        Use with comprehension to obtain subsets:
+
+        >>> from dwopt import pg as d
+        >>> d.create_schema('test')
+        >>> q = d.iris('test.iris', q=1)
+        >>> [i for i in q.cols() if i != 'species']
+        ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
+        """
+        q = "select * from x where 1=2"
+        if out is None:
+            return self.run(q).columns.tolist()
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def dist(self, *args, out=None):
+        """Count number of distinct occurances of data.
+
+        Works on specified columns, or combination of columns, of the sub query table.
+
+        Args
+        ----------
+        *args : str or [str]
+            Either column names as str, or iterator of column name str.
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        pandas.Series
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> q = lt.mtcars(q=1)
+        >>> q.dist('mpg')
+        count(distinct mpg)    25
+        Name: 0, dtype: int64
+        >>> q.dist('mpg', 'cyl')
+        count(distinct mpg)    25
+        count(distinct cyl)     3
+        Name: 0, dtype: int64
+        >>> q.dist(['mpg', 'cyl'])
+        count(distinct mpg || '_' || cyl)    27
+        Name: 0, dtype: int64
+        >>> q.dist(*q.cols()[:4])
+        count(distinct name)    32
+        count(distinct mpg)     25
+        count(distinct cyl)      3
+        count(distinct disp)    27
+        Name: 0, dtype: int64
+
+        >>> from dwopt import pg
+        >>> pg.create_schema('test')
+        >>> q = pg.mtcars('test.mtcars', q=1)
+        >>> q.dist('mpg', ['mpg', 'cyl'], out=1) # doctest: +SKIP
+        with x as (
+            select * from test.mtcars
+        )
+        select
+            count(distinct mpg)
+            ,count(distinct mpg || '_' || cyl)
+        from x
+        >>> q.dist('mpg', ['mpg', 'cyl'])
+        count    25
+        count    27
+        Name: 0, dtype: int64
+        """
+        _ = (" || '_' || ".join(_) if not isinstance(_, str) else _ for _ in args)
+        _ = "".join(
+            f"    ,count(distinct {j})\n" if i else f"    count(distinct {j})\n"
+            for i, j in enumerate(_)
+        )
+        q = "select \n" f"{_}" "from x"
+
+        if out is None:
+            return self.run(q).iloc[0, :]
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def five(self, out=None):
+        """WIP"""
+        raise NotImplementedError
+
+    def from_(self, from_):
+        """Add the from clause to query.
+
+        Alternative to simply specifying table
+        name as the only argument of the qry method. Use the qry method.
+
+        Parameters
+        ----------
+        from_ : str
+            Table name str.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry().from_("iris").print()
+        select * from iris
+        """
+        _ = self.__copy__()
+        _._from_ = from_
+        return _
+
+    def group_by(self, *args):
+        """Add the group by clause to query.
+
+        Parameters
+        ----------
+        *args : str or [str]
+            Group by columns in str format, or iterator of them.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> (
+        ...     lt.qry('mtcars')
+        ...     .select('hp, count(1) n, avg(mpg)')
+        ...     .group_by('hp')
+        ...     .having("avg(mpg) > 30")
+        ...     .run()
+        ... )
+            hp  n  avg(mpg)
+        0   52  1      30.4
+        1   65  1      33.9
+        2  113  1      30.4
+        >>> (
+        ...     lt.qry('mtcars')
+        ...     .select('hp, cyl, count(1) n, avg(mpg)')
+        ...     .group_by('hp,cyl')
+        ...     #.group_by('hp', 'cyl') #same effect
+        ...     #.group_by(['hp', 'cyl']) #same effect
+        ...     .having("avg(mpg) > 30")
+        ...     .print()
+        ... )
+        select hp, cyl, count(1) n, avg(mpg)
+        from mtcars
+        group by hp,cyl
+        having avg(mpg) > 30
+        """
+        _ = self.__copy__()
+        _._group_by = self._args2str(args, ",")
+        return _
+
+    def hash(self, *args, out=None):
+        """Calculate a simple oracle hash for table.
+
+        Arrive at a indicative hash value for a number of columns or all columns of
+        a sub query table.
+        Hash value is a number or symbol that is calculated from data
+        , and is sensitive to any small changes in data. It serves as method to
+        detect if any data element in data is changed.
+
+        Args
+        ----------
+        *args : str or [str]
+            Column names in str. If no value is given, a cols method will be
+            performed to fetch the list of all columns, from which a hash will be
+            calculated.
+            Also allow passing in a single list of str column names.
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        int
+
+        Examples
+        --------
+        ::
+
+            from dwopt import oc
+            q = oc.iris(q=1)
+            q.hash('petal_length')
+            q.hash('petal_length', 'petal_width')
+            q.hash(['petal_length', 'petal_width'])
+            q.hash(out=1)
+        """
+        if self._ops._dialect != "oc":
+            raise NotImplementedError
+        if len(args) == 0:
+            args = self.cols()
+        _ = args[0] if len(args) == 1 and not isinstance(args[0], str) else args
+        _ = " || '_' || ".join(_)
+        q = (
+            "select/*+ PARALLEL(4) */ \n"
+            "    ora_hash(sum(ora_hash(\n"
+            f"        {_}\n"
+            "    ) - 4294967296/2)) hash\n"
+            "from x"
+        )
+        if out is None:
+            return self.run(q).iloc[0, 0]
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def having(self, *args):
+        """Add the having clause to query.
+
+        Parameters
+        ----------
+        *args : str or [str]
+            Conditions in str format, or iterator of them.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> q = (
+        ...     lt.qry('mtcars')
+        ...     .select('hp, count(1) n, avg(mpg)')
+        ...     .group_by('hp')
+        ...     .having("count(1) > 1", "avg(mpg) > 15")
+        ...     .order_by('n desc')
+        ... )
+        >>>
+        >>> q.print()
+        select hp, count(1) n, avg(mpg)
+        from mtcars
+        group by hp
+        having count(1) > 1
+            and avg(mpg) > 15
+        order by n desc
+        >>> q.run()
+            hp  n   avg(mpg)
+        0  180  3  16.300000
+        1  175  3  19.200000
+        2  110  3  21.133333
+        3  150  2  15.350000
+        4  123  2  18.500000
+        5   66  2  29.850000
+        """
+        _ = self.__copy__()
+        _._having = self._args2str(args, "\n    and ")
+        return _
+
+    def head(self, out=None):
+        """Fetch top 5 rows of the sub query table.
+
+        Args
+        -------
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry("iris").head()
+           sepal_length  sepal_width  petal_length  petal_width species
+        0           5.1          3.5           1.4          0.2  setosa
+        1           4.9          3.0           1.4          0.2  setosa
+        2           4.7          3.2           1.3          0.2  setosa
+        3           4.6          3.1           1.5          0.2  setosa
+        4           5.0          3.6           1.4          0.2  setosa
+        """
+        if self._ops._dialect == "oc":
+            q = "select * from x where rownum <= 5"
+        else:
+            q = "select * from x limit 5"
+        if out is None:
+            return self.run(q)
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def join(self, sch_tbl_nme, *args, how="left"):
+        """Add a join clause to query.
+
+        Calling this method multiple times would add multiple clauses.
+
+        Parameters
+        ----------
+        sch_tbl_nme : str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+        *args : str
+            Joining conditions in str format.
+        how : str
+            The join keyword in str format, for example: ``inner``, ``cross``.
+            Default ``left``.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> q = (
+        ...     lt.qry('mtcars a').select('a.cyl, b.mpg')
+        ...     .join('mtcars b','a.name = b.name')
+        ... )
+        >>> q.valc('cyl', 'avg(mpg)')
+           cyl   n   avg(mpg)
+        0    8  14  15.100000
+        1    4  11  26.663636
+        2    6   7  19.742857
+        >>> q.valc('cyl', 'avg(mpg)', out=1) # doctest: +SKIP
+        with x as (
+            select a.cyl, b.mpg
+            from mtcars a
+            left join mtcars b
+                on a.name = b.name
+        )
+        select
+            cyl
+            ,count(1) n
+            ,avg(mpg)
+        from x
+        group by cyl
+        order by n desc
+
+        >>> (
+        ...     lt.qry('mtcars a').select('a.cyl, b.mpg, c.hp')
+        ...     .join('mtcars b','a.name = b.name')
+        ...     .join('mtcars c','a.name = c.name')
+        ...     .valc('cyl', 'avg(mpg), avg(hp)')
+        ... )
+           cyl   n   avg(mpg)     avg(hp)
+        0    8  14  15.100000  209.214286
+        1    4  11  26.663636   82.636364
+        2    6   7  19.742857  122.285714
+
+        Inject a sub-query into the ``sch_tbl_nme`` argument:
+
+        >>> sql = "select cyl from mtcars group by cyl having count(1) > 10"
+        >>> q = (
+        ...     lt.qry('mtcars a').select('a.cyl, a.mpg')
+        ...     .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
+        ... )
+        >>> q.valc('cyl', 'avg(mpg)')
+           cyl   n   avg(mpg)
+        0    8  14  15.100000
+        1    4  11  26.663636
+        >>> q.valc('cyl', 'avg(mpg)', out=1) # doctest: +SKIP
+        with x as (
+            select a.cyl, a.mpg
+            from mtcars a
+            inner join (select cyl from mtcars group by cyl having count(1) > 10) b
+                on a.cyl = b.cyl
+        )
+        select
+            cyl
+            ,count(1) n
+            ,avg(mpg)
+        from x
+        group by cyl
+        order by n desc
+        """
+        _ = self.__copy__()
+        on = self._args2str(args, "\n    and ")
+        cls = f"{how} join {sch_tbl_nme}" f"\n    on {on}"
+        if _._join is not None:
+            _._join = _._join + "\n" + cls
+        else:
+            _._join = cls
+        return _
+
+    def len(self, out=None):
+        """Length of the sub query table.
+
+        Args
+        -------
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        int
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').len()
+        150
+        >>> lt.mtcars(q=1).len()
+        32
+        """
+        q = "select count(1) from x"
+        if out is None:
+            return self.run(q).iloc[0, 0]
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def mimx(self, col, out=None):
+        """Fetch maximum and minimum values of a column.
+
+        Args
+        ----------
+        col : str
+            Column name as str.
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        pandas.Series
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').mimx('sepal_width')
+        max(sepal_width)    4.4
+        min(sepal_width)    2.0
+        Name: 0, dtype: float64
+        """
+        q = "select \n" f"    max({col}),min({col})\n" "from x"
+        if out is None:
+            return self.run(q).iloc[0, :]
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def order_by(self, *args):
+        """
+        Add the order by clause to query.
+
+        Parameters
+        ----------
+        *args : str or [str]
+            Order by names in str format, or iterator of them.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> q = (
+        ...     lt.qry('mtcars')
+        ...     .select('hp, count(1) n, avg(mpg)')
+        ...     .group_by('hp')
+        ...     .having("count(1) > 1", "avg(mpg) > 15")
+        ...     .order_by('n desc')
+        ... )
+        >>>
+        >>> q.run()
+            hp  n   avg(mpg)
+        0  180  3  16.300000
+        1  175  3  19.200000
+        2  110  3  21.133333
+        3  150  2  15.350000
+        4  123  2  18.500000
+        5   66  2  29.850000
+        """
+        _ = self.__copy__()
+        _._order_by = self._args2str(args, ",")
+        return _
+
+    def pct(self):
+        """WIP"""
+        raise NotImplementedError
+
+    def piv(self):
+        """WIP"""
+        raise NotImplementedError
+
+    def print(self, sum_qry=None):
+        """Print the built query.
+
+        * If the ``sum_qry`` argument is not given value,
+          print underlying query as it is.
+        * If a value is given, enclose the underlying query into a with
+          clause, attach the summary query after it, print the full query.
+
+        See also
+        ---------
+        :meth:`dwopt._qry._Qry.str`
+        :meth:`dwopt._qry._Qry.run`
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').select('count(1)').print()
+        select count(1)
+        from iris
+        >>> lt.qry('iris').print('select count(1) from x')
+        with x as (
+            select * from iris
+        )
+        select count(1) from x
+        """
+        print(self.str(sum_qry))
+
+    def run(self, sum_qry=None, **kwargs):
+        """Run the built query.
+
+        * If the ``sum_qry`` argument is not given value,
+          run underlying query as it is.
+        * If a value is given, enclose the underlying query into a with
+          clause, attach the summary query after it, run the full query.
+
+        Args
+        ----------
+        sum_qry: str
+            Summary query string.
+        **kwargs:
+            Keyword arguments to pass on to database operator's run method.
+
+        Returns
+        -------
+        pandas.DataFrame or None
+            Returned by the database operator's
+            :meth:`dwopt.dbo._Db.run` method.
+
+        See also
+        ---------
+        :meth:`dwopt._qry._Qry.str`
+        :meth:`dwopt._qry._Qry.print`
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').select('count(1)').run()
+           count(1)
+        0       150
+        >>> lt.qry('iris').run('select count(1) from x')
+           count(1)
+        0       150
+        >>> lt.qry('iris').where('petal_length>:x').run(
+        ...     'select count(1) from x', mods={'x':2}
+        ... )
+           count(1)
+        0       100
+        """
+        qry = self.str(sum_qry)
+        return self._ops.run(qry, **kwargs)
+
+    def select(self, *args, sep=","):
+        """
+        Add the select clause to query.
+
+        Parameters
+        ----------
+        *args : str or [str]
+            Column name str as positional arguments
+            , or an iterator of str column names.
+        sep : str
+            Symbol used for seperating column names, default ``,``.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> q = lt.iris(q=1)
+        >>> q.select("species, sepal_length").print()
+        select species, sepal_length
+        from iris
+        >>> q.select("species", "sepal_length").print()
+        select species,sepal_length
+        from iris
+        >>> q.select(["species", "sepal_length"]).print()
+        select species,sepal_length
+        from iris
+        >>> q.select(["species", "sepal_length + 2 as sepal_length_new"]).print()
+        select species,sepal_length + 2 as sepal_length_new
+        from iris
+        """
+        _ = self.__copy__()
+        _._select = self._args2str(args, sep)
+        return _
+
+    def sql(self, sql):
+        """Replace the underlying query by specified sql.
+
+        This allows arbituary advanced sql to be incorporated into framework.
+
+        Parameters
+        ----------
+        sql : str
+            Sql code in str format.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> q = lt.qry().sql("select * from iris where sepal_length > 7")
+        >>> q.len()
+        12
+        >>> q.print()
+        select * from iris where sepal_length > 7
+        """
+        _ = self.__copy__()
+        _._sql = sql
+        return _
+
+    def str(self, sum_qry=None):
+        """Return the built query as str.
+
+        * If the ``sum_qry`` argument is not given value,
+          return underlying query as it is.
+        * If a value is given, enclose the underlying query into a with
+          clause, attach the summary query after it, return the full query.
+
+        Args
+        ----------
+        sum_qry: str
+            Summary query string.
+
+        Returns
+        ---------
+        str
+
+        See also
+        ---------
+        :meth:`dwopt._qry._Qry.print`
+        :meth:`dwopt._qry._Qry.run`
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').select('count(1)').str()
+        'select count(1)\\nfrom iris'
+        >>> lt.qry('iris').str('select count(1) from x')
+        'with x as (\\n    select * from iris\\n)\\nselect count(1) from x'
+        """
+        self._make_qry()
+        if sum_qry is not None:
+            _ = self._qry.replace("\n", "\n    ")
+            _ = "with x as (\n" f"    {_}\n" ")"
+            qry = f"{_}\n{sum_qry}"
+        else:
+            qry = self._qry
+        return qry
+
+    def top(self, out=None):
+        """Fetch top row of the sub query table.
+
+        Args
+        -------
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        pandas.Series
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> lt.qry('mtcars').top()
+        name    Mazda RX4
+        mpg          21.0
+        cyl             6
+        disp        160.0
+        hp            110
+        drat          3.9
+        wt           2.62
+        qsec        16.46
+        vs              0
+        am              1
+        gear            4
+        carb            4
+        Name: 0, dtype: object
+
+        Use ``print`` and ``to_string`` to force display of all columns:
+
+        >>> print(lt.iris(q=1).top().to_string())
+        sepal_length       5.1
+        sepal_width        3.5
+        petal_length       1.4
+        petal_width        0.2
+        species         setosa
+        """
+        if self._ops._dialect == "oc":
+            q = "select * from x where rownum<=1"
+        else:
+            q = "select * from x limit 1"
+        if out is None:
+            res = self.run(q)
+            if res.empty:
+                return pd.Series(index=res.columns)
+            else:
+                return res.iloc[0,]
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def valc(self, group_by, agg=None, order_by=None, n=True, out=None):
+        """Value count of a column or combination of columns.
+
+        A value count is a
+        group by query, with total number of row of each group calculated.
+        Also allow custom summary calculation, and custom order by clauses
+        to be added.
+
+        Args
+        ----------
+        group_by : str
+            Group by clause as str.
+        agg : str
+            Custom aggeregation clause as str.
+        order_by : str
+            Order by clause as str.
+        n : Bool
+            Should the value count column be automatically created or not. Default
+            to be True.
+        out: int
+            Output mode. None to run full query, 1 to print full query,
+            2 to return full query as str. Default None.
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Examples
+        --------
+        Various configuration of value counts:
+
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.qry('iris').valc('species', 'avg(petal_length)')
+           species   n  avg(petal_length)
+        0  sicolor  50              4.260
+        1   setosa  50              1.462
+        2  rginica  50              5.552
+        >>> lt.qry('iris').valc('species', 'avg(petal_length) avg', 'avg desc')
+           species   n    avg
+        0  rginica  50  5.552
+        1  sicolor  50  4.260
+        2   setosa  50  1.462
+        >>> lt.qry('iris').valc('species', 'avg(petal_length)', n=False)
+           species  avg(petal_length)
+        0  rginica              5.552
+        1   setosa              1.462
+        2  sicolor              4.260
+        >>> lt.qry('iris').valc('species', 'avg(petal_length)', out=1)# doctest: +SKIP
+        with x as (
+            select * from iris
+        )
+        select
+            species
+            ,count(1) n
+            ,avg(petal_length)
+        from x
+        group by species
+        order by n desc
+
+        Excel-pivot-table-like API:
+
+        .. code-block :: python
+
+            from dwopt import lt, make_test_tbl
+            import logging
+            # logging.basicConfig(level = logging.INFO)
+            _ = make_test_tbl(lt)
+            (
+                lt.qry('test').where('score>0.5', 'dte is not null', 'cat is not null')
+                .valc('dte, cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
+                .pivot('dte', 'cat')
+            )
+
+        Logs showing sql used:
+
+        .. code-block :: sql
+
+            INFO:dwopt.dbo:running:
+            with x as (
+                select * from test
+                where score>0.5
+                    and dte is not null
+                    and cat is not null
+            )
+            select
+                dte, cat
+                ,count(1) n
+                ,avg(score) avgscore, round(sum(amt)/1e3,2) total
+            from x
+            group by dte, cat
+            order by n desc
+            INFO:dwopt.dbo:done
+
+        Results::
+
+                           n        avgscore             total
+            cat         test train      test     train    test   train
+            dte
+            2022-01-01  1140  1051  2.736275  2.800106  565.67  530.09
+            2022-02-02  1077  1100  2.759061  2.748898  536.68  544.10
+            2022-03-03  1037  1072  2.728527  2.743825  521.54  528.85
+
+        Combine case when, value counts, and pivot:
+
+        >>> from dwopt import lt as d
+        >>> d.iris(q=1).case('cat', # doctest: +SKIP
+        ...     "petal_length > 5             then '5+'",
+        ...     "petal_length between 2 and 5 then '2-5'",
+        ...     "petal_length < 2             then '-2'",
+        ... ).valc('species, cat').pivot('species','cat','n')
+        cat        -2   2-5    5+
+        species
+        rginica   NaN   9.0  41.0
+        setosa   50.0   NaN   NaN
+        sicolor   NaN  49.0   1.0
+
+        Make summary for all relevant columns via generated statements:
+
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> q = lt.qry('iris')
+        >>> agg = ', '.join(f'avg({col}) {col}' for col in q.cols() if col != 'species')
+        >>> q.valc('species', agg)
+           species   n  sepal_length  sepal_width  petal_length  petal_width
+        0  sicolor  50         5.936        2.770         4.260        1.326
+        1   setosa  50         5.006        3.428         1.462        0.246
+        2  rginica  50         6.588        2.974         5.552        2.026
+        """
+        group_by_cls = ",".join(group_by) if not isinstance(group_by, str) else group_by
+        if agg is None:
+            agg_cls = ""
+        elif isinstance(agg, str):
+            agg_cls = f"    ,{agg}\n"
+        else:
+            agg_cls = "".join(f"    ,{_}\n" for _ in agg)
+        if order_by is None:
+            if n:
+                order_by_cls = "n desc"
+            else:
+                order_by_cls = group_by_cls
+        else:
+            order_by_cls = order_by
+        q = (
+            "select \n"
+            f"    {group_by_cls}\n"
+            f"{f'    ,count(1) n{chr(10)}' if n else ''}"
+            f"{agg_cls}"
+            "from x\n"
+            f"group by {group_by_cls}\n"
+            f"order by {order_by_cls}"
+        )
+        if out is None:
+            return self.run(q)
+        elif out == 1:
+            self.print(q)
+        elif out == 2:
+            return self.str(q)
+        else:
+            raise ValueError("Invalid out, one of: None, 1, 2")
+
+    def where(self, *args):
+        """
+        Add the where clause to query.
+
+        Parameters
+        ----------
+        *args : str or [str]
+            Conditions in str format, or iterator of condition str.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+            New query object with clause added.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> lt.qry('mtcars').where("cyl = 4").len()
+        11
+        >>> lt.qry('mtcars').where("cyl = 4", "vs = 0").run()
+                    name   mpg  cyl   disp  hp  drat    wt  qsec  vs  am  gear  carb
+        0  Porsche 914-2  26.0    4  120.3  91  4.43  2.14  16.7   0   1     5     2
+        >>> lt.qry('mtcars').where("cyl = 4 and vs = 0").print()
+        select * from mtcars
+        where cyl = 4 and vs = 0
+        """
+        _ = self.__copy__()
+        _._where = self._args2str(args, "\n    and ")
+        return _
```

### Comparing `dwopt-0.0.7/src/dwopt/dbo.py` & `dwopt-0.0.8/src/dwopt/dbo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1314 +1,1334 @@
-import logging
-import re
-
-import numpy as np
-import pandas as pd
-import sqlalchemy as alc
-
-from dwopt._qry import _Qry
-from dwopt.set_up import _make_iris_df, _make_mtcars_df
-
-_logger = logging.getLogger(__name__)
-
-
-def db(eng):
-    """The :class:`database operator object <dwopt.dbo._Db>` factory.
-
-    Args
-    -----------
-    eng: str, or sqlalchemy.engine.Engine
-        A `sqlalchemy engine url <https://docs.sqlalchemy.org/en/14/
-        core/engines.html#database-urls>`_, which
-        combines the user name, password, database names, etc.
-
-        Alternatively a Database connection engine to be used.
-        Use the :func:`dwopt.make_eng` function to make engine.
-
-    Returns
-    -------
-    dwopt.dbo._Db
-        The relevant database operator object.
-
-    Examples
-    -------------
-    Produce a sqlite database operator object:
-
-    >>> from dwopt import db
-    >>> d = db("sqlite://")
-    >>> d.mtcars()
-    >>> d.run('select count(1) from mtcars')
-       count(1)
-    0        32
-
-    Produce a postgre database operator object:
-
-    >>> from dwopt import db
-    >>> url = "postgresql://dwopt_tester:1234@localhost/dwopt_test"
-    >>> db(url).iris(q=True).len()
-    150
-
-    Produce using engine object:
-
-    >>> from dwopt import db, make_eng
-    >>> eng = make_eng("sqlite://")
-    >>> db(eng).mtcars(q=1).len()
-    32
-
-    Produce an oracle database operator object:
-
-    >>> from dwopt import db, Oc
-    >>> url = "oracle://scott2:tiger@tnsname"
-    >>> isinstance(db(url), Oc)
-    True
-    """
-    if isinstance(eng, str):
-        eng = alc.create_engine(eng)
-    else:
-        if not isinstance(eng, alc.engine.Engine):
-            raise ValueError("Invalid eng, either engine url or engine")
-    nme = eng.name
-    if nme == "postgresql":
-        return Pg(eng)
-    elif nme == "sqlite":
-        return Lt(eng)
-    elif nme == "oracle":
-        return Oc(eng)
-    else:
-        raise ValueError("Invalid engine, either postgre, sqlite, or oracle")
-
-
-def Db(eng):
-    """Alias for :func:`dwopt.db`"""
-    return db(eng)
-
-
-class _Db:
-    """
-    The base database operator class.
-
-    See examples for quick-start.
-
-    Instantiate the child classes for different databases via one of below ways:
-
-    * The factory function: :func:`dwopt.db`.
-    * The pre-instantiated objects on package import.
-    * The relevant child classes.
-
-    The child classes and the pre-instantiated objects:
-
-    ========== =================== ========================
-    Database    Child class        Pre-instantiated object
-    ========== =================== ========================
-    Postgre     ``dwopt.Pg(eng)``   ``dwopt.pg``
-    Sqlite      ``dwopt.Lt(eng)``   ``dwopt.lt``
-    Oracle      ``dwopt.Oc(eng)``   ``dwopt.oc``
-    ========== =================== ========================
-
-    Pre-instantiation uses the default credentials set-up prior by the user
-    via the :func:`dwopt.save_url` function.
-
-
-    Args
-    ----------
-    eng: str, or sqlalchemy.engine.Engine
-        A `sqlalchemy engine url <https://docs.sqlalchemy.org/en/14/
-        core/engines.html#database-urls>`_, which
-        combines the user name, password, database names, etc.
-
-        Alternatively a Database connection engine to be used.
-        Use the :func:`dwopt.make_eng` function to make engine.
-
-    Attributes
-    ----------
-    eng: sqlalchemy.engine.Engine
-        Underlying engine. Details see
-        `sqlalchemy.engine.Engine <https://docs.sqlalchemy.org/en/14/core/
-        connections.html#sqlalchemy.engine.Engine>`_
-    meta: sqlalchemy.schema.MetaData
-        Underlying metadata. Details see
-        `sqlalchemy.schema.MetaData <https://docs.sqlalchemy.org/en/14/core/
-        metadata.html#sqlalchemy.schema.MetaData>`_
-
-    Examples
-    --------
-    Instantiate and use a Sqlite database operator object via factory:
-
-    >>> from dwopt import db
-    >>> d = db("sqlite://")
-    >>> d.mtcars()
-    >>> d.run('select count(1) from mtcars')
-       count(1)
-    0        32
-
-    Use the pre-instantiated Sqlite database operator object:
-
-    >>> from dwopt import lt
-    >>> lt.iris()
-    >>> lt.qry('iris').len()
-    150
-
-    Instantiate and use a Postgre database operator object via the class:
-
-    >>> from dwopt import Pg
-    >>> p = Pg("postgresql://dwopt_tester:1234@localhost/dwopt_test")
-    >>> p.mtcars(q=1).len()
-    32
-    """
-
-    def __init__(self, eng):
-        if isinstance(eng, str):
-            self.eng = alc.create_engine(eng)
-        else:
-            self.eng = eng
-        self.meta = alc.MetaData()
-        _nme = self.eng.name
-        if _nme == "postgresql":
-            self._dialect = "pg"
-        elif _nme == "sqlite":
-            self._dialect = "lt"
-        elif _nme == "oracle":
-            self._dialect = "oc"
-
-    def _bind_mods(self, sql, mods=None, **kwargs):
-        """Apply modification to sql statement
-
-        Examples
-        -----------
-        import re
-        def f(sql, i, j):
-            return re.sub(f":{i}(?=[^a-zA-Z0-9]|$)", str(j), sql)
-        f("from tbl_:yr_0304", 'yr', 2017)
-        f(f("from tbl_:yr_:yr1_0304", 'yr', 2017), 'yr1', 2018)
-        f("from tbl_:yr_mth_tbl", 'yr_mth', 2017)
-        """
-        if mods is None:
-            mods = kwargs
-        else:
-            mods.update(kwargs)
-        for i, j in mods.items():
-            sql = re.sub(f":{i}(?=[^a-zA-Z0-9]|$)", str(j), sql)
-            _logger.debug(f"replaced :{i} by {j}")
-        return sql
-
-    def _guess_dtype(self, dtype):
-        """See :meth:`dwopt.dbo._Db.create`"""
-        if self._dialect == "pg":
-            if np.issubdtype(dtype, np.int64):
-                return alc.dialects.postgresql.BIGINT
-            elif np.issubdtype(dtype, np.float64):
-                return alc.Float(8)
-        elif self._dialect == "lt":
-            if np.issubdtype(dtype, np.float64):
-                return alc.REAL
-            elif np.issubdtype(dtype, np.datetime64):
-                return alc.String
-        elif self._dialect == "oc":
-            if np.issubdtype(dtype, np.int64):
-                return alc.dialects.oracle.NUMBER
-            elif np.issubdtype(dtype, np.float64):
-                return alc.Float
-            elif np.issubdtype(dtype, np.datetime64):
-                return alc.Date
-            else:
-                return alc.String(20)
-        else:
-            raise ValueError("invalid dialect, only 'pg', 'lt', or 'oc'")
-
-        if np.issubdtype(dtype, np.int64):
-            return alc.Integer
-        elif np.issubdtype(dtype, np.float64):
-            return alc.Float
-        elif np.issubdtype(dtype, np.datetime64):
-            return alc.DateTime
-        else:
-            return alc.String
-
-    def _parse_sch_tbl_nme(self, sch_tbl_nme, split=True):
-        """Resolve schema dot table name name into lower case components.
-
-        Args
-        ------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-        split: bool
-            Split form or not.
-
-        Returns
-        ----------
-        str or (str, str, str)
-            parsed names, all elements can be None.
-
-        Examples
-        ---------
-        >>> import dwopt
-        >>> d = dwopt.dbo._Db
-        >>> f = lambda x:d._parse_sch_tbl_nme(d, x, split=True)
-        >>> g = lambda x:d._parse_sch_tbl_nme(d, x)
-        >>> for i in ['ab', 'Ab', 'ab.ab', 'Ab.Ab', 'Ab.Ab.Ab', '', None, 3]:
-        ...     print(f"{i = }, {f(i) = }, {g(i) = }")
-        i = 'ab', f(i) = ('ab', None, 'ab'), g(i) = 'ab'
-        i = 'Ab', f(i) = ('ab', None, 'ab'), g(i) = 'ab'
-        i = 'ab.ab', f(i) = ('ab.ab', 'ab', 'ab'), g(i) = 'ab.ab'
-        i = 'Ab.Ab', f(i) = ('ab.ab', 'ab', 'ab'), g(i) = 'ab.ab'
-        i = 'Ab.Ab.Ab', f(i) = ('ab.ab.ab', 'ab', 'ab.ab'), g(i) = 'ab.ab.ab'
-        i = '', f(i) = ('', None, ''), g(i) = ''
-        i = None, f(i) = (None, None, None), g(i) = None
-        i = 3, f(i) = (None, None, None), g(i) = None
-        """
-        try:
-            clean = sch_tbl_nme.lower()
-            items = clean.split(".")
-        except AttributeError:
-            sch = None
-            tbl_nme = None
-            full_nme = None
-        else:
-            n = len(items)
-            if n == 1:
-                sch = None
-                tbl_nme = items[0]
-                full_nme = tbl_nme
-            elif n == 2:
-                sch = items[0]
-                tbl_nme = items[1]
-                full_nme = clean
-            else:
-                sch = items[0]
-                tbl_nme = ".".join(items[1:n])
-                full_nme = clean
-        if split:
-            return full_nme, sch, tbl_nme
-        else:
-            return full_nme
-
-    def _remove_sch_tbl(self, sch_tbl_nme):
-        """Remove sch_tbl from meta.
-
-        Args
-        ------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-
-        Examples
-        -----------
-        Set-up::
-
-            from dwopt import pg
-            import sqlalchemy as alc
-            meta = pg.meta
-
-        First table entry into meta overwrites second one::
-
-            meta.clear()
-            alc.Table('test', meta, schema='test')
-            alc.Table('test.test', meta)
-            meta.tables
-            meta.clear()
-            alc.Table('test.test', meta)
-            alc.Table('test', meta, schema='test')
-            meta.tables
-
-        No schema is entered unless explicitly::
-
-            meta.clear()
-            alc.Table('test.test', meta, schema=None)
-            meta.clear()
-            alc.Table('test.test.test', meta)
-            meta.clear()
-            alc.Table('test.test', meta, schema='test')
-
-        Items removed by key not certain on schema::
-
-            meta.clear()
-            alc.Table('test', meta)
-            alc.Table('test.test', meta)
-            alc.Table('test.test.test', meta)
-            meta.tables['test']
-            meta.tables['test.test']
-            meta.tables['test.test.test']
-            meta.tables
-        """
-        if sch_tbl_nme in self.meta.tables:
-            self.meta.remove(self.meta.tables[sch_tbl_nme])
-
-    def _run(self, sql, args=None):
-        """Run sql statement with argument passing"""
-        with self.eng.begin() as c:
-            _logger.info(f"running:\n{sql}")
-            if args is not None:
-                _logger.info(f"{len(args) = }")
-                r = c.execute(alc.text(sql), args)
-            else:
-                r = c.execute(alc.text(sql))
-            _logger.info("done")
-            if r.returns_rows:
-                return pd.DataFrame(r.all(), columns=r.keys())
-
-    def add_pkey(self, sch_tbl_nme, pkey):
-        """Make and run an add primary key statement.
-
-        Work on postgre and oracle.
-
-        Args
-        ----------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-        pkey : str
-            columns names in form "col1, col2, ...".
-
-        Examples
-        --------
-        >>> from dwopt import pg
-        >>> pg.mtcars()
-        >>> pg.add_pkey('mtcars', 'name')
-        >>> pg.qry('information_schema.constraint_table_usage').select(
-        ...     'table_name, constraint_name').where(
-        ...     "table_schema = 'public'", "table_name = 'mtcars'").run()
-          table_name constraint_name
-        0     mtcars     mtcars_pkey
-        """
-        sql = f"alter table {sch_tbl_nme} add primary key ({pkey})"
-        return self.run(sql)
-
-    def create(self, sch_tbl_nme, dtypes=None, **kwargs):
-        """
-        Make and run a create table statment.
-
-        Args
-        ----------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-        dtypes : {str:str}, optional
-            Dictionary of column names to data types mappings.
-        **kwargs :
-            Convenient way to add mappings.
-            Keyword to argument mappings will be added to the dtypes
-            dictionary.
-
-        Notes
-        -----
-        **Datatypes**
-
-        Datatypes vary across databases
-        (`postgre types <https://www.postgresql.org/docs/current/
-        datatype.html>`_,
-        `sqlite types <https://www.sqlite.org/datatype3.html>`_,
-        `oracle types <https://docs.oracle.com/en/database/oracle/
-        oracle-database/21/sqlqr/Data-Types.html>`_),
-        common example below:
-
-        ========== =========== ======= ============
-        Type       Postgre     Sqlite  Oracle
-        ========== =========== ======= ============
-        integer    bigint      integer number
-        float      float8      real    float
-        string     varchar(20) text    varchar2(20)
-        datetime   timestamp   text    date
-        date       date        text    date
-        ========== =========== ======= ============
-
-        **Other statements**
-
-        The ``dtypes`` mappings also allow other sql statements which are
-        part of a create statement to be added
-        (`sqlite other <https://sqlite.org/lang_createtable.html>`_,
-        `postgre other <https://www.postgresql.org/docs/current/
-        sql-createtable.html>`_,
-        `oracle other <https://docs.oracle.com/en/database/oracle/
-        oracle-database/21/sqlrf/CREATE-TABLE.html>`_).
-        For example a primary key constraint.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.drop('test')
-        >>> lt.create(
-        ...     'test',
-        ...     {
-        ...         'id': 'integer'
-        ...         ,'score': 'real'
-        ...         ,'amt': 'integer'
-        ...         ,'cat': 'text'
-        ...         ,'time': 'text'
-        ...         ,'constraint df_pk': 'primary key (id)'
-        ...     })
-        >>> lt.run("select * from test")
-        Empty DataFrame
-        Columns: [id, score, amt, cat, time]
-        Index: []
-
-        >>> lt.drop('test2')
-        >>> lt.create('test2', id='integer', score='real', cat='text')
-        >>> lt.run("select * from test2")
-        Empty DataFrame
-        Columns: [id, score, cat]
-        Index: []
-        """
-        if dtypes is None:
-            dtypes = kwargs
-        else:
-            dtypes.update(kwargs)
-        cls = ""
-        for col, dtype in dtypes.items():
-            cls += f"\n    ,{col} {dtype}"
-        self.run(f"create table {sch_tbl_nme}(" f"\n    {cls[6:]}" "\n)")
-
-    def create_schema(self, sch_nme):
-        """Make and run a create schema statement.
-
-        Works on postgre.
-
-        Args
-        ----------
-        sch_nme: str
-            Schema name.
-
-        Examples
-        --------
-        >>> from dwopt import pg
-        >>> pg.create_schema('test')
-        >>> pg.iris('test.iris', q=1).len()
-        150
-        """
-        try:
-            self.run(f"create schema {sch_nme}")
-        except Exception as ex:
-            if "already exists" in str(ex):
-                pass
-            else:
-                raise (ex)
-
-    def cwrite(self, df, sch_tbl_nme):
-        """Create table and insert based on dataframe.
-
-        * Replace ``.`` by ``_`` in dataframe column names.
-        * Data types infered based on the :meth:`dwopt.dbo._Db.create` method notes.
-          Also, date type columns are treated same as str type columns.
-        * Reversibility issue see :meth:`dwopt.dbo._Db.write` method notes.
-
-        Args
-        ----------
-        df : pandas.DataFrame
-            Payload Dataframe with data to insert.
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-
-        Examples
-        --------
-        >>> import pandas as pd
-        >>> from dwopt import lt
-        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-        >>> lt.drop('test')
-        >>> lt.cwrite(tbl, 'test')
-        >>> lt.qry('test').run()
-           col1 col2
-        0     1    a
-        1     2    b
-
-        Attempt to write a dataframe into database and query back the same dataframe.
-
-        >>> from dwopt import pg
-        >>> from pandas.testing import assert_frame_equal
-        >>> df = pg.mtcars(q=1).run().sort_values('name').reset_index(drop=True)
-        >>> pg.drop('mtcars2')
-        >>> pg.cwrite(df, 'mtcars2')
-        >>> df_back = pg.qry('mtcars2').run().sort_values('name').reset_index(drop=True)
-        >>> assert_frame_equal(df_back, df)
-        """
-        df = df.copy()
-        df.columns = [_.lower().replace(".", "_") for _ in df.columns]
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        self._remove_sch_tbl(sch_tbl_nme)
-        tbl = alc.Table(
-            tbl_nme,
-            self.meta,
-            *[alc.Column(col, self._guess_dtype(df[col].dtype)) for col in df.columns],
-            schema=sch,
-        )
-        _logger.info("creating table via sqlalchemy:")
-        for col in tbl.columns.items():
-            _logger.info(f"{col}")
-        tbl.create(self.eng)
-        _logger.info("done")
-        self.write(df, sch_tbl_nme)
-
-    def delete(self):
-        """WIP"""
-        raise NotImplementedError
-
-    def drop(self, sch_tbl_nme):
-        """Drop table if exist.
-
-        Args
-        ----------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-
-        See also
-        ----------
-        :meth:`dwopt.dbo._Db.exist`
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.drop('iris')
-        >>> lt.iris()
-        >>> lt.drop('iris')
-        >>> lt.exist('iris')
-        False
-
-        >>> from dwopt import pg
-        >>> pg.create_schema('test')
-        >>> tbl = 'test.iris'
-        >>> pg.iris(tbl)
-        >>> pg.exist(tbl)
-        True
-        >>> pg.drop(tbl)
-        >>> pg.exist(tbl)
-        False
-        """
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        self._remove_sch_tbl(sch_tbl_nme)
-        with self.eng.begin() as conn:
-            _logger.info(f"dropping table via sqlalchemy: {sch_tbl_nme}")
-            alc.Table(tbl_nme, self.meta, schema=sch).drop(conn, checkfirst=True)
-            _logger.info("done")
-
-    def exist(self, sch_tbl_nme):
-        """Check if table exist.
-
-        Args
-        ------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-
-        Returns
-        ----------
-        bool
-
-        Examples
-        ---------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.drop('mtcars')
-        >>> lt.exist('iris')
-        True
-        >>> lt.exist('mtcars')
-        False
-
-        >>> from dwopt import pg as d
-        >>> d.create_schema('test')
-        >>> d.iris('test.iris')
-        >>> d.drop('test.mtcars')
-        >>> d.exist('test.iris')
-        True
-        >>> d.exist('test.mtcars')
-        False
-        """
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        self._remove_sch_tbl(sch_tbl_nme)
-        try:
-            _logger.info(f"reflecting table via sqlalchemy: {sch_tbl_nme}")
-            self.meta.reflect(self.eng, schema=sch, only=[tbl_nme])
-            _logger.info("done")
-            return True
-        except Exception as ex:
-            if "Could not reflect: requested table(s) not available in Engine" in str(
-                ex
-            ):
-                _logger.debug(ex)
-                return False
-            else:
-                raise ex
-
-    def iris(self, sch_tbl_nme="iris", q=False):
-        """Create the iris test table on the database.
-
-        Drop and recreate if already exist.
-        Sourced from `UCI iris <https://archive.ics.uci.edu/ml/datasets/Iris/>`_.
-
-        args
-        -------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-            Default ``iris``.
-        q: bool
-            Return query object or not. Default False.
-
-        Returns
-        -------
-        None or dwopt._qry._Qry
-            Query object with sch_tbl_nme loaded for convenience.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.run('select count(*) from iris')
-           count(*)
-        0       150
-
-        >>> from dwopt import lt
-        >>> lt.iris(q=True).valc('species', 'avg(petal_length)')
-           species   n  avg(petal_length)
-        0  sicolor  50              4.260
-        1   setosa  50              1.462
-        2  rginica  50              5.552
-
-        >>> from dwopt import pg
-        >>> pg.create_schema('test')
-        >>> pg.iris('test.iris', q=1).len()
-        150
-        """
-        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
-        self.drop(sch_tbl_nme)
-        self.cwrite(_make_iris_df(), sch_tbl_nme)
-        if q:
-            return self.qry(sch_tbl_nme)
-
-    def list_cons(self):
-        """
-        List all constraints.
-
-        Only works for postgre.
-        Uses the postgre `information_schema.constraint_table_usage
-        <https://www.postgresql.org/docs/current/infoschema-
-        constraint-table-usage.html>`_ table.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Examples
-        ----------
-        >>> from dwopt import pg
-        >>> pg.mtcars()
-        >>> pg.add_pkey('mtcars', 'name')
-        >>> pg.list_cons().loc[
-        ...     lambda x:(x.table_schema == 'public') & (x.table_name == 'mtcars'),
-        ...     ['table_name', 'constraint_name']
-        ... ].reset_index(drop=True)
-          table_name constraint_name
-        0     mtcars     mtcars_pkey
-        """
-        if self._dialect == "pg":
-            sql = "SELECT * FROM information_schema.constraint_table_usage"
-            return self.run(sql)
-        else:
-            raise NotImplementedError
-
-    def list_tables(self, owner):
-        """
-        List all tables on database or specified schema.
-
-        Args
-        ----------
-        owner : str
-            Only applicable for oracle. Name of the schema(owner).
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Notes
-        -----
-
-        Postgre sql used, `information_schema.tables
-        <https://www.postgresql.org/docs/current/infoschema-tables.html>`_:
-
-        .. code-block:: sql
-
-            select
-                table_catalog,table_schema,table_name
-                ,is_insertable_into,commit_action
-            from information_schema.tables
-            where table_schema
-            not in ('information_schema','pg_catalog')
-
-        Sqlite sql used, `sqlite_schema <https://www.sqlite.org/schematab.html>`_:
-
-        .. code-block:: sql
-
-            select * from sqlite_master
-            where type ='table'
-            and name NOT LIKE 'sqlite_%'
-
-        Oracle sql used, `all_tab_columns
-        <https://docs.oracle.com/en/database/oracle/oracle-database/21/
-        refrn/ALL_TAB_COLUMNS.html>`_:
-
-        .. code-block:: sql
-
-            select/*+PARALLEL (4)*/ owner,table_name
-                ,max(column_name),min(column_name)
-            from all_tab_columns
-            where owner = ':owner'
-            group by owner,table_name
-
-        Examples
-        -----------
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.mtcars()
-        >>> lt.drop('test')
-        >>> lt.drop('test2')
-        >>> lt.list_tables().iloc[:,:-2]
-            type    name tbl_name
-        0  table    iris     iris
-        1  table  mtcars   mtcars
-        """
-        raise NotImplementedError
-
-    def mtcars(self, sch_tbl_nme="mtcars", q=False):
-        """Create the mtcars test table on the database.
-
-        Drop and recreate if already exist.
-        Sourced from `R mtcars <https://www.rdocumentation.org/packages/datasets
-        /versions/3.6.2/topics/mtcars>`_.
-
-        args
-        -------
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-            Default ``mtcars``.
-        q: bool
-            Return query object or not. Default False.
-
-        Returns
-        -------
-        None or dwopt._qry._Qry
-            Query object with sch_tbl_nme loaded for convenience.
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> lt.run('select count(*) from mtcars')
-           count(*)
-        0        32
-
-        >>> from dwopt import lt
-        >>> lt.mtcars(q=True).valc('cyl', 'avg(mpg)')
-           cyl   n   avg(mpg)
-        0    8  14  15.100000
-        1    4  11  26.663636
-        2    6   7  19.742857
-
-        >>> from dwopt import pg
-        >>> pg.create_schema('test')
-        >>> pg.mtcars('test.mtcars', q=1).len()
-        32
-        """
-        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
-        self.drop(sch_tbl_nme)
-        self.cwrite(_make_mtcars_df(), sch_tbl_nme)
-        if q:
-            return self.qry(sch_tbl_nme)
-
-    def qry(self, *args, **kwargs):
-        """Make a :class:`query object <dwopt._qry._Qry>`.
-
-        Args
-        ----------
-        *args :
-            Positional arguments of the :class:`dwopt._qry._Qry`>.
-        **kwargs :
-            keyword arguments of the :class:`dwopt._qry._Qry`.
-
-        Returns
-        -------
-        dwopt._qry._Qry
-
-        Examples
-        --------
-        >>> from dwopt import lt
-        >>> lt.mtcars()
-        >>> lt.qry('mtcars').valc('cyl', 'avg(mpg)')
-           cyl   n   avg(mpg)
-        0    8  14  15.100000
-        1    4  11  26.663636
-        2    6   7  19.742857
-        """
-        return _Qry(self, *args, **kwargs)
-
-    def run(self, sql=None, args=None, pth=None, mods=None, **kwargs):
-        """
-        Run sql statement.
-
-        Features:
-
-        * Argument binding.
-        * Text replacement.
-        * Reading from sql script file.
-
-        Args
-        ----------
-        sql : str, optional
-            The sql statement to run.
-        args : dict, or [dict], optional
-            Dictionary or list of dictionary of argument name str to argument
-            data object mappings.
-            These argument data objects are passed via sqlalchemy to the database,
-            to function as data for the argument names.
-            See the notes and the examples section for details.
-        pth : str, optional
-            Path to sql script, ignored if the sql parameter is not None.
-            The script can hold a sql statement, for example a significant piece
-            of table creation statement.
-        mods : dict, optional
-            Dictionary of modification name str to modification str mappings.
-            Replaces modification name in the sql by the respective
-            modification str.
-            See the notes and the examples section for details.
-        **kwargs :
-            Convenient way to add modification mappings.
-            Keyword to argument mappings will be added to the mods dictionary.
-            The keyword cannot be one of the positional parameter names.
-
-        Returns
-        -------
-        pandas.DataFrame or None
-            Returns dataframe if the database returns any result.
-            Returns dataframe with column names and zero rows if running query
-            that returns zero rows.
-            Returns None otherwise, typically when running DDL/DML statement.
-
-        Notes
-        -----
-
-        **The args and the mods parameter**
-
-        An argument name or a modification name is denoted in the sql by prepending
-        a colon symbol ``:`` before a series of alphanumeric or underscore symbols.
-
-        In addition, the end of the series for the modification name is to be
-        followed by a non-alphanumeric or a end of line symbol. This is to distinguish
-        names such as ``:var`` and ``:var1``.
-
-        The args parameter binding is recommanded where possible,
-        while the mods paramter method of text replacement gives
-        more flexibility when it comes to programatically generate sql statment.
-
-        Examples
-        --------
-        Run sql:
-
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.run("select * from iris limit 1")
-           sepal_length  sepal_width  petal_length  petal_width species
-        0           5.1          3.5           1.4          0.2  setosa
-
-        Run sql with argument passing:
-
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> lt.run("select count(1) from iris where species = :x",
-        ...     args = {'x':'setosa'})
-           count(1)
-        0        50
-
-        Run sql with text modification:
-
-        >>> from dwopt import lt
-        >>> lt.iris()
-        >>> old = 'iris'
-        >>> new = 'iris2'
-        >>> lt.run("drop table if exists :var", var=new)
-        >>> lt.run("create table :x as select * from :y", mods={'x':new, 'y': old})
-        >>> lt.run("select count(1) from :tbl", tbl=new)
-           count(1)
-        0       150
-
-        Run from sql script:
-
-        >>> from dwopt import pg, make_test_tbl
-        >>> _ = make_test_tbl(pg)
-        >>> pg.run(pth = "E:/projects/my_sql_script.sql", # doctest: +SKIP
-        ...     my_run_dte = '2022-03-03',
-        ...     my_label = '20220303',
-        ...     threshold = 5)
-           count
-        0    137
-
-        Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
-
-        .. code-block:: sql
-
-            drop table if exists monthly_extract_:my_label;
-
-            create table monthly_extract_:my_label as
-            select * from test
-            where
-                dte = to_date(':my_run_dte','YYYY-MM-DD')
-                and score > :threshold;
-
-            select count(1) from monthly_extract_:my_label;
-
-        """
-        if sql is None and pth is not None:
-            with open(pth) as f:
-                sql = f.read()
-            _logger.info(f"sql from:\n{pth}")
-        if mods is not None or len(kwargs) > 0:
-            sql = self._bind_mods(sql, mods, **kwargs)
-        return self._run(sql, args)
-
-    def table_cols(self, sch_tbl_nme):
-        """
-        Show information of specified table's columns.
-
-        Notes
-        -----
-
-        Postgre sql used, `information_schema.columns
-        <https://www.postgresql.org/docs/current/infoschema-columns.html>`_:
-
-        .. code-block:: sql
-
-            select column_name, data_type
-            from information_schema.columns
-            where table_schema = ':schema_nme'
-            and table_name = ':tbl_nme'
-
-        Oracle sql used, `all_tab_columns
-        <https://docs.oracle.com/en/database/oracle/oracle-database/21/
-        refrn/ALL_TAB_COLUMNS.html>`_:
-
-        .. code-block:: sql
-
-            select/*+PARALLEL (4)*/ *
-            from all_tab_columns
-            where owner = ':schema_nme'
-            and table_name = ':tbl_nme'
-
-        Parameters
-        ----------
-        sch_tbl_nme : str
-            Table name in format: `schema.table`.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Examples
-        -----------
-        >>> from dwopt import pg
-        >>> pg.iris()
-        >>> pg.table_cols('public.iris')
-            column_name          data_type
-        0  sepal_length               real
-        1   sepal_width               real
-        2  petal_length               real
-        3   petal_width               real
-        4       species  character varying
-        """
-        raise NotImplementedError
-
-    def table_sizes(self):
-        """
-        List sizes of all tables in current schema.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-        Notes
-        -----
-
-        Oracle sql used, `user_extents
-        <https://docs.oracle.com/en/database/oracle/oracle-database/21/refrn/
-        USER_EXTENTS.html>`_:
-
-        .. code-block:: sql
-
-            select/*+PARALLEL (4)*/
-                tablespace_name,segment_type,segment_name
-                ,sum(bytes)/1024/1024 table_size_mb
-            from user_extents
-            group by tablespace_name,segment_type,segment_name
-
-        """
-        raise NotImplementedError
-
-    def update(self):
-        """WIP"""
-        raise NotImplementedError
-
-    def write(self, df, sch_tbl_nme):
-        """Make and run a insert many statement.
-
-        **Pre-processing**
-
-        * Pandas Datetime64 columns are converted into object columns, and the
-          ``pandas.NaT`` objects are converted into ``None``.
-        * Pandas Float64 columns are converted into object columns, and the
-          ``pandas.NaN`` objects are converted into ``None``.
-
-        This should follow from a :meth:`dwopt.dbo._Db.create` call which sets up
-        the database table with table name, column names, intended data types,
-        and constraints.
-
-        Args
-        ----------
-        df: pandas.DataFrame
-            Payload Dataframe with data to insert.
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-
-        Notes
-        -----
-
-        **Reversibility**
-
-        Ideally python dataframe written to database should allow a exact same
-        dataframe to be read back into python. Whether this is true depends on:
-
-        * The database.
-        * The data and object types on the dataframe.
-        * The data types on the database table.
-
-        With the set up used in the :func:`dwopt.make_test_tbl` function,
-        following results is obtained:
-
-        * The postgre table is reversible except for row order on select from database.
-          Example fix/strategy for comparison:
-
-          .. code-block:: python
-
-              df.sort_values('id').reset_index(drop=True)
-
-        * Sqlite stores date/datetime as text, this causes a str type column to
-          be read back. One strategy is to convert from datatime and NaT to
-          str and None before insertion, and convert to date and datetime
-          when reading back.
-          Example fix/strategy for comparison:
-
-          .. code-block:: python
-
-              lt.write(
-                  df.assign(
-                      time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
-                  "test2",
-              )
-              tbl = (
-                  db.qry("test2").run()
-                  .assign(
-                      dte=lambda x: x["dte"].apply(
-                          lambda x: datetime.date.fromisoformat(x) if x else None
-                      ),
-                      time=lambda x: pd.to_datetime(x.time),
-                  )
-              )
-
-        * Oracle has same issue as postgre. In addition:
-
-          * Both date and datetime are stored as date format, and are read back
-            as datetime.
-          * Datetime milliseconds are lost on the database.
-          * Date are stored in dd-MMM-yy format on database.
-          * Date passed into varchar2 type column are stored in dd-MMM-yy format.
-
-          Example fix/strategy for comparison:
-
-          .. code-block:: python
-
-              tbl = db.run("select * from test2 order by id").assign(
-                  dte=lambda x: x["dte"].apply(lambda x: x.date() if x else None)
-              )
-              df2 = df.assign(
-                  time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
-              )
-
-        Examples
-        --------
-        Write dataframe into a table.
-
-        >>> import pandas as pd
-        >>> from dwopt import lt
-        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-        >>> lt.drop('test')
-        >>> lt.create('test', col1='int', col2='text')
-        >>> lt.write(tbl,'test')
-        >>> lt.run('select * from test')
-           col1 col2
-        0     1    a
-        1     2    b
-
-        Attempt to write a dataframe into database and query back the same dataframe.
-
-        >>> from dwopt import make_test_tbl
-        >>> from pandas.testing import assert_frame_equal
-        >>> pg, df = make_test_tbl('pg')
-        >>> pg.drop('test')
-        >>> pg.create(
-        ...     "test",
-        ...     dtypes={
-        ...         "id": "bigint primary key",
-        ...         "score": "float8",
-        ...         "amt": "bigint",
-        ...         "cat": "varchar(20)",
-        ...         "dte":"date",
-        ...         "time":"timestamp"
-        ...     }
-        ... )
-        >>> pg.write(df, 'test')
-        >>> df_back = pg.qry('test').run().sort_values('id').reset_index(drop=True)
-        >>> assert_frame_equal(df_back, df)
-        """
-        L = len(df)
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        if L == 0:
-            return
-        df = df.copy()
-        cols = df.columns.tolist()
-        for col in cols:
-            if np.issubdtype(df[col].dtype, np.datetime64) or np.issubdtype(
-                df[col].dtype, np.float64
-            ):
-                df[col] = df[col].astype(object).where(~df[col].isna(), None)
-        self._remove_sch_tbl(sch_tbl_nme)
-        tbl = alc.Table(
-            tbl_nme, self.meta, *[alc.Column(col) for col in cols], schema=sch
-        )
-        _logger.info(f"running:\n{tbl.insert()}")
-        _ = df.to_dict("records")
-        _logger.info(f"args len={L}, e.g.\n{_[0]}")
-        with self.eng.begin() as conn:
-            conn.execute(
-                tbl.insert(),
-                _,
-            )
-        _logger.info("done")
-
-    def write_nodup(self, tbl, sch_tbl_nme, pkey, where=None):
-        """Insert without creating duplicates.
-
-        Does below:
-
-        1. Make and run a select statement with optionally provided
-           where clause.
-        2. If step 1 returns any results and the payload table in non-empty
-           , remove duplicates on the payload table, using the provided primary
-           key columns as judge of duplication.
-        3. Make insert statement on the non-duplicating payload data via the
-           :meth:`dwopt.dbo._Db.write` method.
-
-        Args
-        ----------
-        tbl: pandas.DataFrame
-            Payload Dataframe with data to insert.
-        sch_tbl_nme: str
-            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-        pkey: [str]
-            Iterable of column name str.
-        where: str
-            where clause in str form. The ``where`` keyword is not needed.
-
-        See also
-        --------
-        :meth:`dwopt.dbo._Db.write`
-
-        Examples
-        --------
-        >>> import pandas as pd
-        >>> from dwopt import lt
-        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-        >>> tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
-        >>> lt.drop('test')
-        >>> lt.create('test', col1='int', col2='text')
-        >>> lt.write(tbl, 'test')
-        >>> lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
-        >>> lt.run("select * from test")
-           col1 col2
-        0     1    a
-        1     2    b
-        2     3    c
-        """
-        cols = ",".join(pkey)
-        where_cls = f"\nwhere {where}" if where else ""
-        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
-        db_tbl = self.run(f"select {cols} from {sch_tbl_nme} {where_cls}")
-        l_tbl = len(tbl)
-        l_db_tbl = len(db_tbl)
-        if l_tbl > 0 and l_db_tbl > 0:
-            dedup_tbl = (
-                tbl.merge(
-                    db_tbl, how="left", on=pkey, validate="one_to_one", indicator=True
-                )
-                .loc[lambda x: x._merge == "left_only", :]
-                .drop(columns="_merge")
-            )
-        else:
-            dedup_tbl = tbl
-        _logger.debug(
-            f"write nodup: {l_tbl = }, {l_db_tbl = }" f", {len(dedup_tbl) = }"
-        )
-        self.write(dedup_tbl, sch_tbl_nme)
-
-
-class Pg(_Db):
-    def list_cons(self):
-        sql = "SELECT * FROM information_schema.constraint_table_usage"
-        return self.run(sql)
-
-    def list_tables(self):
-        sql = (
-            "select table_catalog,table_schema,table_name"
-            "\n    ,is_insertable_into,commit_action"
-            "\nfrom information_schema.tables"
-            "\nwhere table_schema"
-            "\n   not in ('information_schema','pg_catalog')"
-        )
-        return self.run(sql)
-
-    def table_cols(self, sch_tbl_nme):
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        sql = (
-            "select column_name, data_type from information_schema.columns"
-            f"\nwhere table_schema = '{sch}' "
-            f"\nand table_name = '{tbl_nme}'"
-        )
-        return self.run(sql)
-
-
-class Lt(_Db):
-    def list_tables(self):
-        sql = (
-            "select * from sqlite_master "
-            "\nwhere type ='table' "
-            "\nand name NOT LIKE 'sqlite_%' "
-        )
-        return self.run(sql)
-
-
-class Oc(_Db):
-    def list_tables(self, owner):
-        sql = (
-            "select/*+PARALLEL (4)*/ owner,table_name"
-            "\n    ,max(column_name),min(column_name)"
-            "\nfrom all_tab_columns"
-            f"\nwhere owner = '{owner.upper()}'"
-            "\ngroup by owner,table_name"
-        )
-        return self.run(sql)
-
-    def table_cols(self, sch_tbl_nme):
-        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
-        sql = (
-            "select/*+PARALLEL (4)*/ *"
-            "\nfrom all_tab_columns"
-            f"\nwhere owner = '{sch.upper()}'"
-            f"\nand table_name = '{tbl_nme.upper()}'"
-        )
-        return self.run(sql)
-
-    def table_sizes(self):
-        sql = (
-            "select/*+PARALLEL (4)*/"
-            "\n    tablespace_name,segment_type,segment_name"
-            "\n    ,sum(bytes)/1024/1024 table_size_mb"
-            "\nfrom user_extents"
-            "\ngroup by tablespace_name,segment_type,segment_name"
-        )
-        return self.run(sql)
+import logging
+import re
+
+import numpy as np
+import pandas as pd
+import sqlalchemy as alc
+
+from dwopt._qry import _Qry
+from dwopt.set_up import _make_iris_df, _make_mtcars_df
+
+_logger = logging.getLogger(__name__)
+
+
+def db(eng, **kwargs):
+    """The :class:`database operator object <dwopt.dbo._Db>` factory.
+
+    Args
+    -----------
+    eng: str, or sqlalchemy.engine.Engine
+        A `sqlalchemy engine url <https://docs.sqlalchemy.org/en/14/
+        core/engines.html#database-urls>`_, which
+        combines the user name, password, database names, etc.
+
+        Alternatively a Database connection engine to be used.
+        Use the :func:`dwopt.make_eng` function to make engine.
+
+    kwargs: Additional engine creation arguments.
+
+    Returns
+    -------
+    dwopt.dbo._Db
+        The relevant database operator object.
+
+    Examples
+    -------------
+    Produce a sqlite database operator object:
+
+    >>> from dwopt import db
+    >>> d = db("sqlite://")
+    >>> d.mtcars()
+    >>> d.run('select count(1) from mtcars')
+       count(1)
+    0        32
+
+    Produce a postgre database operator object:
+
+    >>> from dwopt import db
+    >>> url = "postgresql://dwopt_tester:1234@localhost/dwopt_test"
+    >>> db(url).iris(q=True).len()
+    150
+
+    Produce using engine object:
+
+    >>> from dwopt import db, make_eng
+    >>> eng = make_eng("sqlite://")
+    >>> db(eng).mtcars(q=1).len()
+    32
+
+    Produce an oracle database operator object:
+
+    >>> from dwopt import db, Oc
+    >>> url = "oracle+oracledb://scott2:tiger@tnsname"
+    >>> isinstance(db(url), Oc)
+    True
+
+    Use additional engine creation arguments::
+
+        from dwopt import db
+        url = (
+            "oracle+oracledb://dwopt_test:1234@localhost:1521/?service_name=XEPDB1 "
+            "&encoding=UTF-8&nencoding=UTF-8"
+        )
+        lib_dir = "C:/app/{user_name}/product/21c/dbhomeXE/bin"
+        o = db(url, thick_mode={"lib_dir": lib_dir})
+        o.run("select * from dual")
+    """
+    if isinstance(eng, str):
+        eng = alc.create_engine(eng, **kwargs)
+    else:
+        if not isinstance(eng, alc.engine.Engine):
+            raise ValueError("Invalid eng, either engine url or engine")
+    nme = eng.name
+    if nme == "postgresql":
+        return Pg(eng)
+    elif nme == "sqlite":
+        return Lt(eng)
+    elif nme == "oracle":
+        return Oc(eng)
+    else:
+        raise ValueError("Invalid engine, either postgres, sqlite, or oracle")
+
+
+def Db(eng, **kwargs):
+    """Alias for :func:`dwopt.db`"""
+    return db(eng, **kwargs)
+
+
+class _Db:
+    """
+    The base database operator class.
+
+    See examples for quick-start.
+
+    Instantiate the child classes for different databases via one of below ways:
+
+    * The factory function: :func:`dwopt.db`.
+    * The pre-instantiated objects on package import.
+    * The relevant child classes.
+
+    The child classes and the pre-instantiated objects:
+
+    ========== =================== ========================
+    Database    Child class        Pre-instantiated object
+    ========== =================== ========================
+    Postgre     ``dwopt.Pg(eng)``   ``dwopt.pg``
+    Sqlite      ``dwopt.Lt(eng)``   ``dwopt.lt``
+    Oracle      ``dwopt.Oc(eng)``   ``dwopt.oc``
+    ========== =================== ========================
+
+    Pre-instantiation uses the default credentials set-up prior by the user
+    via the :func:`dwopt.save_url` function.
+
+
+    Args
+    ----------
+    eng: str, or sqlalchemy.engine.Engine
+        A `sqlalchemy engine url <https://docs.sqlalchemy.org/en/14/
+        core/engines.html#database-urls>`_, which
+        combines the user name, password, database names, etc.
+
+        Alternatively a Database connection engine to be used.
+        Use the :func:`dwopt.make_eng` function to make engine.
+    kwargs: Additional engine creation arguments.
+
+    Attributes
+    ----------
+    eng: sqlalchemy.engine.Engine
+        Underlying engine. Details see
+        `sqlalchemy.engine.Engine <https://docs.sqlalchemy.org/en/14/core/
+        connections.html#sqlalchemy.engine.Engine>`_
+    meta: sqlalchemy.schema.MetaData
+        Underlying metadata. Details see
+        `sqlalchemy.schema.MetaData <https://docs.sqlalchemy.org/en/14/core/
+        metadata.html#sqlalchemy.schema.MetaData>`_
+
+    Examples
+    --------
+    Instantiate and use a Sqlite database operator object via factory:
+
+    >>> from dwopt import db
+    >>> d = db("sqlite://")
+    >>> d.mtcars()
+    >>> d.run('select count(1) from mtcars')
+       count(1)
+    0        32
+
+    Use the pre-instantiated Sqlite database operator object:
+
+    >>> from dwopt import lt
+    >>> lt.iris()
+    >>> lt.qry('iris').len()
+    150
+
+    Instantiate and use a Postgre database operator object via the class:
+
+    >>> from dwopt import Pg
+    >>> p = Pg("postgresql://dwopt_tester:1234@localhost/dwopt_test")
+    >>> p.mtcars(q=1).len()
+    32
+
+    Additonal engine creation arguments::
+
+        from dwopt import Pg
+        p = Pg("postgresql://dwopt_tester:1234@localhost/dwopt_test", echo=1)
+        p.mtcars()
+    """
+
+    def __init__(self, eng, **kwargs):
+        if isinstance(eng, str):
+            self.eng = alc.create_engine(eng, **kwargs)
+        else:
+            self.eng = eng
+        self.meta = alc.MetaData()
+        _nme = self.eng.name
+        if _nme == "postgresql":
+            self._dialect = "pg"
+        elif _nme == "sqlite":
+            self._dialect = "lt"
+        elif _nme == "oracle":
+            self._dialect = "oc"
+
+    def _bind_mods(self, sql, mods=None, **kwargs):
+        """Apply modification to sql statement
+
+        Examples
+        -----------
+        import re
+        def f(sql, i, j):
+            return re.sub(f":{i}(?=[^a-zA-Z0-9]|$)", str(j), sql)
+        f("from tbl_:yr_0304", 'yr', 2017)
+        f(f("from tbl_:yr_:yr1_0304", 'yr', 2017), 'yr1', 2018)
+        f("from tbl_:yr_mth_tbl", 'yr_mth', 2017)
+        """
+        if mods is None:
+            mods = kwargs
+        else:
+            mods.update(kwargs)
+        for i, j in mods.items():
+            sql = re.sub(f":{i}(?=[^a-zA-Z0-9]|$)", str(j), sql)
+            _logger.debug(f"replaced :{i} by {j}")
+        return sql
+
+    def _guess_dtype(self, dtype):
+        """See :meth:`dwopt.dbo._Db.create`"""
+        if self._dialect == "pg":
+            if np.issubdtype(dtype, np.int64):
+                return alc.dialects.postgresql.BIGINT
+            elif np.issubdtype(dtype, np.float64):
+                return alc.Float(8)
+        elif self._dialect == "lt":
+            if np.issubdtype(dtype, np.float64):
+                return alc.REAL
+            elif np.issubdtype(dtype, np.datetime64):
+                return alc.String
+        elif self._dialect == "oc":
+            if np.issubdtype(dtype, np.int64):
+                return alc.dialects.oracle.NUMBER
+            elif np.issubdtype(dtype, np.float64):
+                return alc.Float
+            elif np.issubdtype(dtype, np.datetime64):
+                return alc.Date
+            else:
+                return alc.String(20)
+        else:
+            raise ValueError("invalid dialect, only 'pg', 'lt', or 'oc'")
+
+        if np.issubdtype(dtype, np.int64):
+            return alc.Integer
+        elif np.issubdtype(dtype, np.float64):
+            return alc.Float
+        elif np.issubdtype(dtype, np.datetime64):
+            return alc.DateTime
+        else:
+            return alc.String
+
+    def _parse_sch_tbl_nme(self, sch_tbl_nme, split=True):
+        """Resolve schema dot table name name into lower case components.
+
+        Args
+        ------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+        split: bool
+            Split form or not.
+
+        Returns
+        ----------
+        str or (str, str, str)
+            parsed names, all elements can be None.
+
+        Examples
+        ---------
+        >>> import dwopt
+        >>> d = dwopt.dbo._Db
+        >>> f = lambda x:d._parse_sch_tbl_nme(d, x, split=True)
+        >>> g = lambda x:d._parse_sch_tbl_nme(d, x)
+        >>> for i in ['ab', 'Ab', 'ab.ab', 'Ab.Ab', 'Ab.Ab.Ab', '', None, 3]:
+        ...     print(f"{i = }, {f(i) = }, {g(i) = }")
+        i = 'ab', f(i) = ('ab', None, 'ab'), g(i) = 'ab'
+        i = 'Ab', f(i) = ('ab', None, 'ab'), g(i) = 'ab'
+        i = 'ab.ab', f(i) = ('ab.ab', 'ab', 'ab'), g(i) = 'ab.ab'
+        i = 'Ab.Ab', f(i) = ('ab.ab', 'ab', 'ab'), g(i) = 'ab.ab'
+        i = 'Ab.Ab.Ab', f(i) = ('ab.ab.ab', 'ab', 'ab.ab'), g(i) = 'ab.ab.ab'
+        i = '', f(i) = ('', None, ''), g(i) = ''
+        i = None, f(i) = (None, None, None), g(i) = None
+        i = 3, f(i) = (None, None, None), g(i) = None
+        """
+        try:
+            clean = sch_tbl_nme.lower()
+            items = clean.split(".")
+        except AttributeError:
+            sch = None
+            tbl_nme = None
+            full_nme = None
+        else:
+            n = len(items)
+            if n == 1:
+                sch = None
+                tbl_nme = items[0]
+                full_nme = tbl_nme
+            elif n == 2:
+                sch = items[0]
+                tbl_nme = items[1]
+                full_nme = clean
+            else:
+                sch = items[0]
+                tbl_nme = ".".join(items[1:n])
+                full_nme = clean
+        if split:
+            return full_nme, sch, tbl_nme
+        else:
+            return full_nme
+
+    def _remove_sch_tbl(self, sch_tbl_nme):
+        """Remove sch_tbl from meta.
+
+        Args
+        ------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+
+        Examples
+        -----------
+        Set-up::
+
+            from dwopt import pg
+            import sqlalchemy as alc
+            meta = pg.meta
+
+        First table entry into meta overwrites second one::
+
+            meta.clear()
+            alc.Table('test', meta, schema='test')
+            alc.Table('test.test', meta)
+            meta.tables
+            meta.clear()
+            alc.Table('test.test', meta)
+            alc.Table('test', meta, schema='test')
+            meta.tables
+
+        No schema is entered unless explicitly::
+
+            meta.clear()
+            alc.Table('test.test', meta, schema=None)
+            meta.clear()
+            alc.Table('test.test.test', meta)
+            meta.clear()
+            alc.Table('test.test', meta, schema='test')
+
+        Items removed by key not certain on schema::
+
+            meta.clear()
+            alc.Table('test', meta)
+            alc.Table('test.test', meta)
+            alc.Table('test.test.test', meta)
+            meta.tables['test']
+            meta.tables['test.test']
+            meta.tables['test.test.test']
+            meta.tables
+        """
+        if sch_tbl_nme in self.meta.tables:
+            self.meta.remove(self.meta.tables[sch_tbl_nme])
+
+    def _run(self, sql, args=None):
+        """Run sql statement with argument passing"""
+        with self.eng.begin() as c:
+            _logger.info(f"running:\n{sql}")
+            if args is not None:
+                _logger.info(f"{len(args) = }")
+                r = c.execute(alc.text(sql), args)
+            else:
+                r = c.execute(alc.text(sql))
+            _logger.info("done")
+            if r.returns_rows:
+                return pd.DataFrame(r.all(), columns=r.keys())
+
+    def add_pkey(self, sch_tbl_nme, pkey):
+        """Make and run an add primary key statement.
+
+        Work on postgre and oracle.
+
+        Args
+        ----------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+        pkey : str
+            columns names in form "col1, col2, ...".
+
+        Examples
+        --------
+        >>> from dwopt import pg
+        >>> pg.mtcars()
+        >>> pg.add_pkey('mtcars', 'name')
+        >>> pg.qry('information_schema.constraint_table_usage').select(
+        ...     'table_name, constraint_name').where(
+        ...     "table_schema = 'public'", "table_name = 'mtcars'").run()
+          table_name constraint_name
+        0     mtcars     mtcars_pkey
+        """
+        sql = f"alter table {sch_tbl_nme} add primary key ({pkey})"
+        return self.run(sql)
+
+    def create(self, sch_tbl_nme, dtypes=None, **kwargs):
+        """
+        Make and run a create table statment.
+
+        Args
+        ----------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+        dtypes : {str:str}, optional
+            Dictionary of column names to data types mappings.
+        **kwargs :
+            Convenient way to add mappings.
+            Keyword to argument mappings will be added to the dtypes
+            dictionary.
+
+        Notes
+        -----
+        **Datatypes**
+
+        Datatypes vary across databases
+        (`postgre types <https://www.postgresql.org/docs/current/
+        datatype.html>`_,
+        `sqlite types <https://www.sqlite.org/datatype3.html>`_,
+        `oracle types <https://docs.oracle.com/en/database/oracle/
+        oracle-database/21/sqlqr/Data-Types.html>`_),
+        common example below:
+
+        ========== =========== ======= ============
+        Type       Postgre     Sqlite  Oracle
+        ========== =========== ======= ============
+        integer    bigint      integer number
+        float      float8      real    float
+        string     varchar(20) text    varchar2(20)
+        datetime   timestamp   text    date
+        date       date        text    date
+        ========== =========== ======= ============
+
+        **Other statements**
+
+        The ``dtypes`` mappings also allow other sql statements which are
+        part of a create statement to be added
+        (`sqlite other <https://sqlite.org/lang_createtable.html>`_,
+        `postgre other <https://www.postgresql.org/docs/current/
+        sql-createtable.html>`_,
+        `oracle other <https://docs.oracle.com/en/database/oracle/
+        oracle-database/21/sqlrf/CREATE-TABLE.html>`_).
+        For example a primary key constraint.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.drop('test')
+        >>> lt.create(
+        ...     'test',
+        ...     {
+        ...         'id': 'integer'
+        ...         ,'score': 'real'
+        ...         ,'amt': 'integer'
+        ...         ,'cat': 'text'
+        ...         ,'time': 'text'
+        ...         ,'constraint df_pk': 'primary key (id)'
+        ...     })
+        >>> lt.run("select * from test")
+        Empty DataFrame
+        Columns: [id, score, amt, cat, time]
+        Index: []
+
+        >>> lt.drop('test2')
+        >>> lt.create('test2', id='integer', score='real', cat='text')
+        >>> lt.run("select * from test2")
+        Empty DataFrame
+        Columns: [id, score, cat]
+        Index: []
+        """
+        if dtypes is None:
+            dtypes = kwargs
+        else:
+            dtypes.update(kwargs)
+        cls = ""
+        for col, dtype in dtypes.items():
+            cls += f"\n    ,{col} {dtype}"
+        self.run(f"create table {sch_tbl_nme}(" f"\n    {cls[6:]}" "\n)")
+
+    def create_schema(self, sch_nme):
+        """Make and run a create schema statement.
+
+        Works on postgre.
+
+        Args
+        ----------
+        sch_nme: str
+            Schema name.
+
+        Examples
+        --------
+        >>> from dwopt import pg
+        >>> pg.create_schema('test')
+        >>> pg.iris('test.iris', q=1).len()
+        150
+        """
+        try:
+            self.run(f"create schema {sch_nme}")
+        except Exception as ex:
+            if "already exists" in str(ex):
+                pass
+            else:
+                raise (ex)
+
+    def cwrite(self, df, sch_tbl_nme):
+        """Create table and insert based on dataframe.
+
+        * Replace ``.`` by ``_`` in dataframe column names.
+        * Data types infered based on the :meth:`dwopt.dbo._Db.create` method notes.
+          Also, date type columns are treated same as str type columns.
+        * Reversibility issue see :meth:`dwopt.dbo._Db.write` method notes.
+
+        Args
+        ----------
+        df : pandas.DataFrame
+            Payload Dataframe with data to insert.
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> from dwopt import lt
+        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+        >>> lt.drop('test')
+        >>> lt.cwrite(tbl, 'test')
+        >>> lt.qry('test').run()
+           col1 col2
+        0     1    a
+        1     2    b
+
+        Attempt to write a dataframe into database and query back the same dataframe.
+
+        >>> from dwopt import pg
+        >>> from pandas.testing import assert_frame_equal
+        >>> df = pg.mtcars(q=1).run().sort_values('name').reset_index(drop=True)
+        >>> pg.drop('mtcars2')
+        >>> pg.cwrite(df, 'mtcars2')
+        >>> df_back = pg.qry('mtcars2').run().sort_values('name').reset_index(drop=True)
+        >>> assert_frame_equal(df_back, df)
+        """
+        df = df.copy()
+        df.columns = [_.lower().replace(".", "_") for _ in df.columns]
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        self._remove_sch_tbl(sch_tbl_nme)
+        tbl = alc.Table(
+            tbl_nme,
+            self.meta,
+            *[alc.Column(col, self._guess_dtype(df[col].dtype)) for col in df.columns],
+            schema=sch,
+        )
+        _logger.info("creating table via sqlalchemy:")
+        for col in tbl.columns.items():
+            _logger.info(f"{col}")
+        tbl.create(self.eng)
+        _logger.info("done")
+        self.write(df, sch_tbl_nme)
+
+    def delete(self):
+        """WIP"""
+        raise NotImplementedError
+
+    def drop(self, sch_tbl_nme):
+        """Drop table if exist.
+
+        Args
+        ----------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+
+        See also
+        ----------
+        :meth:`dwopt.dbo._Db.exist`
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.drop('iris')
+        >>> lt.iris()
+        >>> lt.drop('iris')
+        >>> lt.exist('iris')
+        False
+
+        >>> from dwopt import pg
+        >>> pg.create_schema('test')
+        >>> tbl = 'test.iris'
+        >>> pg.iris(tbl)
+        >>> pg.exist(tbl)
+        True
+        >>> pg.drop(tbl)
+        >>> pg.exist(tbl)
+        False
+        """
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        self._remove_sch_tbl(sch_tbl_nme)
+        with self.eng.begin() as conn:
+            _logger.info(f"dropping table via sqlalchemy: {sch_tbl_nme}")
+            alc.Table(tbl_nme, self.meta, schema=sch).drop(conn, checkfirst=True)
+            _logger.info("done")
+
+    def exist(self, sch_tbl_nme):
+        """Check if table exist.
+
+        Args
+        ------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+
+        Returns
+        ----------
+        bool
+
+        Examples
+        ---------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.drop('mtcars')
+        >>> lt.exist('iris')
+        True
+        >>> lt.exist('mtcars')
+        False
+
+        >>> from dwopt import pg as d
+        >>> d.create_schema('test')
+        >>> d.iris('test.iris')
+        >>> d.drop('test.mtcars')
+        >>> d.exist('test.iris')
+        True
+        >>> d.exist('test.mtcars')
+        False
+        """
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        self._remove_sch_tbl(sch_tbl_nme)
+        try:
+            _logger.info(f"reflecting table via sqlalchemy: {sch_tbl_nme}")
+            self.meta.reflect(self.eng, schema=sch, only=[tbl_nme])
+            _logger.info("done")
+            return True
+        except Exception as ex:
+            if "Could not reflect: requested table(s) not available in Engine" in str(
+                ex
+            ):
+                _logger.debug(ex)
+                return False
+            else:
+                raise ex
+
+    def iris(self, sch_tbl_nme="iris", q=False):
+        """Create the iris test table on the database.
+
+        Drop and recreate if already exist.
+        Sourced from `UCI iris <https://archive.ics.uci.edu/ml/datasets/Iris/>`_.
+
+        args
+        -------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+            Default ``iris``.
+        q: bool
+            Return query object or not. Default False.
+
+        Returns
+        -------
+        None or dwopt._qry._Qry
+            Query object with sch_tbl_nme loaded for convenience.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.run('select count(*) from iris')
+           count(*)
+        0       150
+
+        >>> from dwopt import lt
+        >>> lt.iris(q=True).valc('species', 'avg(petal_length)')
+           species   n  avg(petal_length)
+        0  sicolor  50              4.260
+        1   setosa  50              1.462
+        2  rginica  50              5.552
+
+        >>> from dwopt import pg
+        >>> pg.create_schema('test')
+        >>> pg.iris('test.iris', q=1).len()
+        150
+        """
+        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
+        self.drop(sch_tbl_nme)
+        self.cwrite(_make_iris_df(), sch_tbl_nme)
+        if q:
+            return self.qry(sch_tbl_nme)
+
+    def list_cons(self):
+        """
+        List all constraints.
+
+        Only works for postgre.
+        Uses the postgre `information_schema.constraint_table_usage
+        <https://www.postgresql.org/docs/current/infoschema-
+        constraint-table-usage.html>`_ table.
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Examples
+        ----------
+        >>> from dwopt import pg
+        >>> pg.mtcars()
+        >>> pg.add_pkey('mtcars', 'name')
+        >>> pg.list_cons().loc[
+        ...     lambda x:(x.table_schema == 'public') & (x.table_name == 'mtcars'),
+        ...     ['table_name', 'constraint_name']
+        ... ].reset_index(drop=True)
+          table_name constraint_name
+        0     mtcars     mtcars_pkey
+        """
+        if self._dialect == "pg":
+            sql = "SELECT * FROM information_schema.constraint_table_usage"
+            return self.run(sql)
+        else:
+            raise NotImplementedError
+
+    def list_tables(self, owner):
+        """
+        List all tables on database or specified schema.
+
+        Args
+        ----------
+        owner : str
+            Only applicable for oracle. Name of the schema(owner).
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Notes
+        -----
+
+        Postgre sql used, `information_schema.tables
+        <https://www.postgresql.org/docs/current/infoschema-tables.html>`_:
+
+        .. code-block:: sql
+
+            select
+                table_catalog,table_schema,table_name
+                ,is_insertable_into,commit_action
+            from information_schema.tables
+            where table_schema
+            not in ('information_schema','pg_catalog')
+
+        Sqlite sql used, `sqlite_schema <https://www.sqlite.org/schematab.html>`_:
+
+        .. code-block:: sql
+
+            select * from sqlite_master
+            where type ='table'
+            and name NOT LIKE 'sqlite_%'
+
+        Oracle sql used, `all_tab_columns
+        <https://docs.oracle.com/en/database/oracle/oracle-database/21/
+        refrn/ALL_TAB_COLUMNS.html>`_:
+
+        .. code-block:: sql
+
+            select/*+PARALLEL (4)*/ owner,table_name
+                ,max(column_name),min(column_name)
+            from all_tab_columns
+            where owner = ':owner'
+            group by owner,table_name
+
+        Examples
+        -----------
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.mtcars()
+        >>> lt.drop('test')
+        >>> lt.drop('test2')
+        >>> lt.list_tables().iloc[:,:-2]
+            type    name tbl_name
+        0  table    iris     iris
+        1  table  mtcars   mtcars
+        """
+        raise NotImplementedError
+
+    def mtcars(self, sch_tbl_nme="mtcars", q=False):
+        """Create the mtcars test table on the database.
+
+        Drop and recreate if already exist.
+        Sourced from `R mtcars <https://www.rdocumentation.org/packages/datasets
+        /versions/3.6.2/topics/mtcars>`_.
+
+        args
+        -------
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+            Default ``mtcars``.
+        q: bool
+            Return query object or not. Default False.
+
+        Returns
+        -------
+        None or dwopt._qry._Qry
+            Query object with sch_tbl_nme loaded for convenience.
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> lt.run('select count(*) from mtcars')
+           count(*)
+        0        32
+
+        >>> from dwopt import lt
+        >>> lt.mtcars(q=True).valc('cyl', 'avg(mpg)')
+           cyl   n   avg(mpg)
+        0    8  14  15.100000
+        1    4  11  26.663636
+        2    6   7  19.742857
+
+        >>> from dwopt import pg
+        >>> pg.create_schema('test')
+        >>> pg.mtcars('test.mtcars', q=1).len()
+        32
+        """
+        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
+        self.drop(sch_tbl_nme)
+        self.cwrite(_make_mtcars_df(), sch_tbl_nme)
+        if q:
+            return self.qry(sch_tbl_nme)
+
+    def qry(self, *args, **kwargs):
+        """Make a :class:`query object <dwopt._qry._Qry>`.
+
+        Args
+        ----------
+        *args :
+            Positional arguments of the :class:`dwopt._qry._Qry`>.
+        **kwargs :
+            keyword arguments of the :class:`dwopt._qry._Qry`.
+
+        Returns
+        -------
+        dwopt._qry._Qry
+
+        Examples
+        --------
+        >>> from dwopt import lt
+        >>> lt.mtcars()
+        >>> lt.qry('mtcars').valc('cyl', 'avg(mpg)')
+           cyl   n   avg(mpg)
+        0    8  14  15.100000
+        1    4  11  26.663636
+        2    6   7  19.742857
+        """
+        return _Qry(self, *args, **kwargs)
+
+    def run(self, sql=None, args=None, pth=None, mods=None, **kwargs):
+        """
+        Run sql statement.
+
+        Features:
+
+        * Argument binding.
+        * Text replacement.
+        * Reading from sql script file.
+
+        Args
+        ----------
+        sql : str, optional
+            The sql statement to run.
+        args : dict, or [dict], optional
+            Dictionary or list of dictionary of argument name str to argument
+            data object mappings.
+            These argument data objects are passed via sqlalchemy to the database,
+            to function as data for the argument names.
+            See the notes and the examples section for details.
+        pth : str, optional
+            Path to sql script, ignored if the sql parameter is not None.
+            The script can hold a sql statement, for example a significant piece
+            of table creation statement.
+        mods : dict, optional
+            Dictionary of modification name str to modification str mappings.
+            Replaces modification name in the sql by the respective
+            modification str.
+            See the notes and the examples section for details.
+        **kwargs :
+            Convenient way to add modification mappings.
+            Keyword to argument mappings will be added to the mods dictionary.
+            The keyword cannot be one of the positional parameter names.
+
+        Returns
+        -------
+        pandas.DataFrame or None
+            Returns dataframe if the database returns any result.
+            Returns dataframe with column names and zero rows if running query
+            that returns zero rows.
+            Returns None otherwise, typically when running DDL/DML statement.
+
+        Notes
+        -----
+
+        **The args and the mods parameter**
+
+        An argument name or a modification name is denoted in the sql by prepending
+        a colon symbol ``:`` before a series of alphanumeric or underscore symbols.
+
+        In addition, the end of the series for the modification name is to be
+        followed by a non-alphanumeric or a end of line symbol. This is to distinguish
+        names such as ``:var`` and ``:var1``.
+
+        The args parameter binding is recommanded where possible,
+        while the mods paramter method of text replacement gives
+        more flexibility when it comes to programatically generate sql statment.
+
+        Examples
+        --------
+        Run sql:
+
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.run("select * from iris limit 1")
+           sepal_length  sepal_width  petal_length  petal_width species
+        0           5.1          3.5           1.4          0.2  setosa
+
+        Run sql with argument passing:
+
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> lt.run("select count(1) from iris where species = :x",
+        ...     args = {'x':'setosa'})
+           count(1)
+        0        50
+
+        Run sql with text modification:
+
+        >>> from dwopt import lt
+        >>> lt.iris()
+        >>> old = 'iris'
+        >>> new = 'iris2'
+        >>> lt.run("drop table if exists :var", var=new)
+        >>> lt.run("create table :x as select * from :y", mods={'x':new, 'y': old})
+        >>> lt.run("select count(1) from :tbl", tbl=new)
+           count(1)
+        0       150
+
+        Run from sql script:
+
+        >>> from dwopt import pg, make_test_tbl
+        >>> _ = make_test_tbl(pg)
+        >>> pg.run(pth = "E:/projects/my_sql_script.sql", # doctest: +SKIP
+        ...     my_run_dte = '2022-03-03',
+        ...     my_label = '20220303',
+        ...     threshold = 5)
+           count
+        0    137
+
+        Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
+
+        .. code-block:: sql
+
+            drop table if exists monthly_extract_:my_label;
+
+            create table monthly_extract_:my_label as
+            select * from test
+            where
+                dte = to_date(':my_run_dte','YYYY-MM-DD')
+                and score > :threshold;
+
+            select count(1) from monthly_extract_:my_label;
+
+        """
+        if sql is None and pth is not None:
+            with open(pth) as f:
+                sql = f.read()
+            _logger.info(f"sql from:\n{pth}")
+        if mods is not None or len(kwargs) > 0:
+            sql = self._bind_mods(sql, mods, **kwargs)
+        return self._run(sql, args)
+
+    def table_cols(self, sch_tbl_nme):
+        """
+        Show information of specified table's columns.
+
+        Notes
+        -----
+
+        Postgre sql used, `information_schema.columns
+        <https://www.postgresql.org/docs/current/infoschema-columns.html>`_:
+
+        .. code-block:: sql
+
+            select column_name, data_type
+            from information_schema.columns
+            where table_schema = ':schema_nme'
+            and table_name = ':tbl_nme'
+
+        Oracle sql used, `all_tab_columns
+        <https://docs.oracle.com/en/database/oracle/oracle-database/21/
+        refrn/ALL_TAB_COLUMNS.html>`_:
+
+        .. code-block:: sql
+
+            select/*+PARALLEL (4)*/ *
+            from all_tab_columns
+            where owner = ':schema_nme'
+            and table_name = ':tbl_nme'
+
+        Parameters
+        ----------
+        sch_tbl_nme : str
+            Table name in format: `schema.table`.
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Examples
+        -----------
+        >>> from dwopt import pg
+        >>> pg.iris()
+        >>> pg.table_cols('public.iris')
+            column_name          data_type
+        0  sepal_length               real
+        1   sepal_width               real
+        2  petal_length               real
+        3   petal_width               real
+        4       species  character varying
+        """
+        raise NotImplementedError
+
+    def table_sizes(self):
+        """
+        List sizes of all tables in current schema.
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Notes
+        -----
+
+        Oracle sql used, `user_extents
+        <https://docs.oracle.com/en/database/oracle/oracle-database/21/refrn/
+        USER_EXTENTS.html>`_:
+
+        .. code-block:: sql
+
+            select/*+PARALLEL (4)*/
+                tablespace_name,segment_type,segment_name
+                ,sum(bytes)/1024/1024 table_size_mb
+            from user_extents
+            group by tablespace_name,segment_type,segment_name
+
+        """
+        raise NotImplementedError
+
+    def update(self):
+        """WIP"""
+        raise NotImplementedError
+
+    def write(self, df, sch_tbl_nme):
+        """Make and run a insert many statement.
+
+        **Pre-processing**
+
+        * Pandas Datetime64 columns are converted into object columns, and the
+          ``pandas.NaT`` objects are converted into ``None``.
+        * Pandas Float64 columns are converted into object columns, and the
+          ``pandas.NaN`` objects are converted into ``None``.
+
+        This should follow from a :meth:`dwopt.dbo._Db.create` call which sets up
+        the database table with table name, column names, intended data types,
+        and constraints.
+
+        Args
+        ----------
+        df: pandas.DataFrame
+            Payload Dataframe with data to insert.
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+
+        Notes
+        -----
+
+        **Reversibility**
+
+        Ideally python dataframe written to database should allow a exact same
+        dataframe to be read back into python. Whether this is true depends on:
+
+        * The database.
+        * The data and object types on the dataframe.
+        * The data types on the database table.
+
+        With the set up used in the :func:`dwopt.make_test_tbl` function,
+        following results is obtained:
+
+        * The postgre table is reversible except for row order on select from database.
+          Example fix/strategy for comparison:
+
+          .. code-block:: python
+
+              df.sort_values('id').reset_index(drop=True)
+
+        * Sqlite stores date/datetime as text, this causes a str type column to
+          be read back. One strategy is to convert from datatime and NaT to
+          str and None before insertion, and convert to date and datetime
+          when reading back.
+          Example fix/strategy for comparison:
+
+          .. code-block:: python
+
+              lt.write(
+                  df.assign(
+                      time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
+                  "test2",
+              )
+              tbl = (
+                  db.qry("test2").run()
+                  .assign(
+                      dte=lambda x: x["dte"].apply(
+                          lambda x: datetime.date.fromisoformat(x) if x else None
+                      ),
+                      time=lambda x: pd.to_datetime(x.time),
+                  )
+              )
+
+        * Oracle has same issue as postgre. In addition:
+
+          * Both date and datetime are stored as date format, and are read back
+            as datetime.
+          * Datetime milliseconds are lost on the database.
+          * Date are stored in dd-MMM-yy format on database.
+          * Date passed into varchar2 type column are stored in dd-MMM-yy format.
+
+          Example fix/strategy for comparison:
+
+          .. code-block:: python
+
+              tbl = db.run("select * from test2 order by id").assign(
+                  dte=lambda x: x["dte"].apply(lambda x: x.date() if x else None)
+              )
+              df2 = df.assign(
+                  time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
+              )
+
+        Examples
+        --------
+        Write dataframe into a table.
+
+        >>> import pandas as pd
+        >>> from dwopt import lt
+        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+        >>> lt.drop('test')
+        >>> lt.create('test', col1='int', col2='text')
+        >>> lt.write(tbl,'test')
+        >>> lt.run('select * from test')
+           col1 col2
+        0     1    a
+        1     2    b
+
+        Attempt to write a dataframe into database and query back the same dataframe.
+
+        >>> from dwopt import make_test_tbl
+        >>> from pandas.testing import assert_frame_equal
+        >>> pg, df = make_test_tbl('pg')
+        >>> pg.drop('test')
+        >>> pg.create(
+        ...     "test",
+        ...     dtypes={
+        ...         "id": "bigint primary key",
+        ...         "score": "float8",
+        ...         "amt": "bigint",
+        ...         "cat": "varchar(20)",
+        ...         "dte":"date",
+        ...         "time":"timestamp"
+        ...     }
+        ... )
+        >>> pg.write(df, 'test')
+        >>> df_back = pg.qry('test').run().sort_values('id').reset_index(drop=True)
+        >>> assert_frame_equal(df_back, df)
+        """
+        L = len(df)
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        if L == 0:
+            return
+        df = df.copy()
+        cols = df.columns.tolist()
+        for col in cols:
+            if np.issubdtype(df[col].dtype, np.datetime64) or np.issubdtype(
+                df[col].dtype, np.float64
+            ):
+                df[col] = df[col].astype(object).where(~df[col].isna(), None)
+        self._remove_sch_tbl(sch_tbl_nme)
+        tbl = alc.Table(
+            tbl_nme, self.meta, *[alc.Column(col) for col in cols], schema=sch
+        )
+        _logger.info(f"running:\n{tbl.insert()}")
+        _ = df.to_dict("records")
+        _logger.info(f"args len={L}, e.g.\n{_[0]}")
+        with self.eng.begin() as conn:
+            conn.execute(
+                tbl.insert(),
+                _,
+            )
+        _logger.info("done")
+
+    def write_nodup(self, tbl, sch_tbl_nme, pkey, where=None):
+        """Insert without creating duplicates.
+
+        Does below:
+
+        1. Make and run a select statement with optionally provided
+           where clause.
+        2. If step 1 returns any results and the payload table in non-empty
+           , remove duplicates on the payload table, using the provided primary
+           key columns as judge of duplication.
+        3. Make insert statement on the non-duplicating payload data via the
+           :meth:`dwopt.dbo._Db.write` method.
+
+        Args
+        ----------
+        tbl: pandas.DataFrame
+            Payload Dataframe with data to insert.
+        sch_tbl_nme: str
+            Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+        pkey: [str]
+            Iterable of column name str.
+        where: str
+            where clause in str form. The ``where`` keyword is not needed.
+
+        See also
+        --------
+        :meth:`dwopt.dbo._Db.write`
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> from dwopt import lt
+        >>> tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+        >>> tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
+        >>> lt.drop('test')
+        >>> lt.create('test', col1='int', col2='text')
+        >>> lt.write(tbl, 'test')
+        >>> lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
+        >>> lt.run("select * from test")
+           col1 col2
+        0     1    a
+        1     2    b
+        2     3    c
+        """
+        cols = ",".join(pkey)
+        where_cls = f"\nwhere {where}" if where else ""
+        sch_tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme, split=False)
+        db_tbl = self.run(f"select {cols} from {sch_tbl_nme} {where_cls}")
+        l_tbl = len(tbl)
+        l_db_tbl = len(db_tbl)
+        if l_tbl > 0 and l_db_tbl > 0:
+            dedup_tbl = (
+                tbl.merge(
+                    db_tbl, how="left", on=pkey, validate="one_to_one", indicator=True
+                )
+                .loc[lambda x: x._merge == "left_only", :]
+                .drop(columns="_merge")
+            )
+        else:
+            dedup_tbl = tbl
+        _logger.debug(
+            f"write nodup: {l_tbl = }, {l_db_tbl = }" f", {len(dedup_tbl) = }"
+        )
+        self.write(dedup_tbl, sch_tbl_nme)
+
+
+class Pg(_Db):
+    def list_cons(self):
+        sql = "SELECT * FROM information_schema.constraint_table_usage"
+        return self.run(sql)
+
+    def list_tables(self):
+        sql = (
+            "select table_catalog,table_schema,table_name"
+            "\n    ,is_insertable_into,commit_action"
+            "\nfrom information_schema.tables"
+            "\nwhere table_schema"
+            "\n   not in ('information_schema','pg_catalog')"
+        )
+        return self.run(sql)
+
+    def table_cols(self, sch_tbl_nme):
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        sql = (
+            "select column_name, data_type from information_schema.columns"
+            f"\nwhere table_schema = '{sch}' "
+            f"\nand table_name = '{tbl_nme}'"
+        )
+        return self.run(sql)
+
+
+class Lt(_Db):
+    def list_tables(self):
+        sql = (
+            "select * from sqlite_master "
+            "\nwhere type ='table' "
+            "\nand name NOT LIKE 'sqlite_%' "
+        )
+        return self.run(sql)
+
+
+class Oc(_Db):
+    def list_tables(self, owner):
+        sql = (
+            "select/*+PARALLEL (4)*/ owner,table_name"
+            "\n    ,max(column_name),min(column_name)"
+            "\nfrom all_tab_columns"
+            f"\nwhere owner = '{owner.upper()}'"
+            "\ngroup by owner,table_name"
+        )
+        return self.run(sql)
+
+    def table_cols(self, sch_tbl_nme):
+        sch_tbl_nme, sch, tbl_nme = self._parse_sch_tbl_nme(sch_tbl_nme)
+        sql = (
+            "select/*+PARALLEL (4)*/ *"
+            "\nfrom all_tab_columns"
+            f"\nwhere owner = '{sch.upper()}'"
+            f"\nand table_name = '{tbl_nme.upper()}'"
+        )
+        return self.run(sql)
+
+    def table_sizes(self):
+        sql = (
+            "select/*+PARALLEL (4)*/"
+            "\n    tablespace_name,segment_type,segment_name"
+            "\n    ,sum(bytes)/1024/1024 table_size_mb"
+            "\nfrom user_extents"
+            "\ngroup by tablespace_name,segment_type,segment_name"
+        )
+        return self.run(sql)
```

### Comparing `dwopt-0.0.7/src/dwopt/testing.py` & `dwopt-0.0.8/src/dwopt/testing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,285 +1,287 @@
-import datetime
-import random
-
-import pandas as pd
-import sqlalchemy as alc
-
-import dwopt
-from dwopt.set_up import _TEST_LT_URL, _TEST_OC_URL, _TEST_PG_URL
-
-
-def _make_test_df(n=10000):
-    random.seed(0)
-    df = pd.DataFrame(
-        {
-            "id": range(n),
-            "score": [random.uniform(-1, 5) for i in range(n)],
-            "amt": random.choices(range(1000), k=n),
-            "cat": random.choices(["test", "train"], k=n),
-            "dte": [
-                datetime.date.fromisoformat(i)
-                for i in random.choices(["2022-01-01", "2022-02-02", "2022-03-03"], k=n)
-            ],
-            "time": [
-                datetime.datetime.fromisoformat(i)
-                for i in random.choices(
-                    [
-                        "2022-01-01 00:19:02.011135",
-                        "2022-02-02 23:00:00.000000",
-                        "2022-03-03 10:19:35.071235",
-                    ],
-                    k=n,
-                )
-            ],
-        }
-    )
-
-    for col in ["score", "cat", "dte", "time"]:
-        df.loc[random.choices(range(n), k=int(n / 20)), col] = None
-
-    return df
-
-
-def _parse_sch_tbl_nme(sch_tbl_nme):
-    db = dwopt.dbo._Db
-    return db._parse_sch_tbl_nme(db, sch_tbl_nme)
-
-
-def _make_pg_tbl(df, eng, sch_tbl_nme):
-    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
-    meta = alc.MetaData()
-    test_tbl = alc.Table(
-        tbl_nme,
-        meta,
-        alc.Column("id", alc.dialects.postgresql.BIGINT, primary_key=True),
-        alc.Column("score", alc.Float(8)),
-        alc.Column("amt", alc.dialects.postgresql.BIGINT),
-        alc.Column("cat", alc.String(20)),
-        alc.Column("dte", alc.Date),
-        alc.Column("time", alc.DateTime),
-        schema=sch,
-    )
-    with eng.begin() as conn:
-        test_tbl.drop(conn, checkfirst=True)
-    meta.create_all(eng)
-    with eng.begin() as conn:
-        conn.execute(
-            test_tbl.insert(),
-            df.assign(
-                time=lambda x: x.time.astype(object).where(~x.time.isna(), None)
-            ).to_dict("records"),
-        )
-
-
-def _make_lt_tbl(df, eng, sch_tbl_nme):
-    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
-    meta = alc.MetaData()
-    test_tbl = alc.Table(
-        tbl_nme,
-        meta,
-        alc.Column("id", alc.Integer, primary_key=True),
-        alc.Column("score", alc.REAL),
-        alc.Column("amt", alc.Integer),
-        alc.Column("cat", alc.String),
-        alc.Column("dte", alc.String),
-        alc.Column("time", alc.String),
-        schema=sch,
-    )
-    with eng.begin() as conn:
-        test_tbl.drop(conn, checkfirst=True)
-    meta.create_all(eng)
-    with eng.begin() as conn:
-        conn.execute(
-            test_tbl.insert(),
-            df.assign(
-                time=lambda x: x.time.astype(str).where(~x.time.isna(), None)
-            ).to_dict("records"),
-        )
-
-
-def _make_oc_tbl(df, eng, sch_tbl_nme):
-    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
-    meta = alc.MetaData()
-    test_tbl = alc.Table(
-        tbl_nme,
-        meta,
-        alc.Column("id", alc.dialects.oracle.NUMBER, primary_key=True),
-        alc.Column("score", alc.Float),
-        alc.Column("amt", alc.dialects.oracle.NUMBER),
-        alc.Column("cat", alc.String(20)),
-        alc.Column("dte", alc.Date),
-        alc.Column("time", alc.Date),
-        schema=sch,
-    )
-    with eng.begin() as conn:
-        test_tbl.drop(conn, checkfirst=True)
-    meta.create_all(eng)
-    with eng.begin() as conn:
-        conn.execute(
-            test_tbl.insert(),
-            df.assign(
-                score=lambda x: x.score.astype(object).where(~x.score.isna(), None),
-                time=lambda x: x.time.astype(object).where(~x.time.isna(), None),
-            ).to_dict("records"),
-        )
-
-
-def make_test_tbl(db, sch_tbl_nme="test", n=10000):
-    """Make or remake a test table on database.
-
-    Uses Sqlalchemy toolkits for table drop, creation, insertion.
-
-    Parameters
-    ------------
-    db: dwopt.dbo._Db, or str
-        Dwopt database operator object. Or one of ``'pg'``, ``'lt'``, and ``'oc'``,
-        indicating usage of pre-defined testing database engines.
-    sch_tbl_nme: str
-        Table name in form ``my_schema1.my_table1`` or ``my_table1``.
-    n: int
-        Number of records.
-
-    Returns
-    ----------
-    (dwopt.dbo._Db, pandas.DataFrame):
-        Tuple of database operator used, and the test dataframe.
-
-    Notes
-    ------
-
-    **Table specifications**
-
-    ====== ============== ============== ==== ===================
-    Column Column type    Object type    None Example
-    ====== ============== ============== ==== ===================
-    id     int64          int64               0
-    score  float64        float64        NaN  4.066531
-    amt    int64          int64               867
-    cat    object         str            None train
-    dte    object         datetime.date  None 2022-03-03
-    time   datetime64[ns] datetime64[ns] NaT  2022-02-02 23:00:00
-    ====== ============== ============== ==== ===================
-
-    **Test database table specifications**
-
-    ====== =========== ======= ============
-    Column Postgre     Sqlite  Oracle
-    ====== =========== ======= ============
-    id     bigint      integer number
-    score  float8      real    float
-    amt    bigint      integer number
-    cat    varchar(20) text    varchar2(20)
-    dte    date        text    date
-    time   timestamp   text    date
-    ====== =========== ======= ============
-
-    These datatypes are implemented via closest
-    `Sqlalchemy datatypes <https://docs.sqlalchemy.org/en/14/core/type_basics.html>`_.
-
-    The ``id`` column is made primary key in the test database tables.
-
-    *Floating point types*
-
-    The ``score`` column's ``NaN`` objects are converted into ``None`` before insertion
-    for oracle.
-
-    *Datetime types*
-
-    The ``time`` column's ``NaT`` objects are converted into ``None`` before insertion
-    for Postgre and Oracle.
-    The ``time`` column are converted into str and None before insertion for Sqlite.
-
-    **Pre-defined testing database engines**
-
-    * ``pg``: ``postgresql://dwopt_tester:1234@localhost/dwopt_test``
-    * ``lt``: ``sqlite://``
-    * ``oc``: ``oracle://dwopt_test:1234@localhost:1521/?service_name=XEPDB1
-      &encoding=UTF-8&nencoding=UTF-8``.
-
-    **Install testing databases**
-
-    *Postgre*
-
-    * Install from
-      `postgresql windows <https://www.postgresql.org/download/windows/>`_.
-    * Add postgres bin directory to path.
-    * Run commands:
-
-      .. code-block:: console
-
-        psql -U postgres
-        CREATE DATABASE dwopt_test;
-        CREATE USER dwopt_tester WITH PASSWORD '1234';
-        GRANT ALL PRIVILEGES ON DATABASE dwopt_test to dwopt_tester;
-
-    *Postgre on linux*
-
-    .. code-block:: console
-
-        sudo su postgres
-        psql
-        CREATE DATABASE dwopt_test;
-        CREATE USER dwopt_tester WITH PASSWORD '1234';
-        GRANT ALL PRIVILEGES ON DATABASE dwopt_test to dwopt_tester;
-
-    *Oracle*
-
-    * Install from
-      `oracle xe <https://www.oracle.com/database/technologies/xe-downloads.html>`_.
-    * Set ORACLE_HOME, ORACLE_SID environment variable, and path based on the
-      `oracle configuration <https://docs.oracle.com/database/121/ADMQS/
-      GUID-EC18C4A6-3BA5-4C14-9D76-B0DD62FEFFF2.htm#ADMQS12369>`_.
-    * Run commands:
-
-      .. code-block:: console
-
-        sqlplus sys/{PASSWORD}@//localhost:1521/XEPDB1 as sysdba
-        create user dwopt_test identified by 1234;
-        grant create session to dwopt_test;
-        grant create table to dwopt_test;
-        grant unlimited tablespace to dwopt_test;
-
-    Examples
-    ----------
-    Make test table via provided database operator:
-
-    >>> from dwopt import lt, make_test_tbl
-    >>> _ = make_test_tbl(lt)
-    >>> lt.qry('test').len()
-    10000
-
-    Make database operator for the pre-defined test databases,
-    then make test table on it:
-
-    >>> from dwopt import make_test_tbl
-    >>> lt, df = make_test_tbl('lt', 'foo', 999)
-    >>> lt.eng
-    Engine(sqlite://)
-    >>> lt.qry('foo').len()
-    999
-    >>> len(df)
-    999
-    """
-    if isinstance(db, str):
-        if db == "pg":
-            db = dwopt.db(_TEST_PG_URL)
-        elif db == "lt":
-            db = dwopt.db(_TEST_LT_URL)
-        elif db == "oc":
-            db = dwopt.db(_TEST_OC_URL)
-        else:
-            raise ValueError("Invalid db str, use one of 'pg', 'lt', or 'oc'")
-    df = _make_test_df(n)
-    dlc = db._dialect
-    if dlc == "pg":
-        _make_pg_tbl(df, db.eng, sch_tbl_nme)
-    elif dlc == "lt":
-        _make_lt_tbl(df, db.eng, sch_tbl_nme)
-    elif dlc == "oc":
-        _make_oc_tbl(df, db.eng, sch_tbl_nme)
-    else:
-        raise ValueError(
-            "Invalid db, must be a database operator object, instances of "
-            "(dwopt.Pg, dwopt.Lt, dwopt.Oc)"
-        )
-    return db, df
+import datetime
+import random
+
+import pandas as pd
+import sqlalchemy as alc
+
+import dwopt
+from dwopt.set_up import _TEST_LT_URL, _TEST_OC_URL, _TEST_PG_URL
+
+
+def _make_test_df(n=10000):
+    random.seed(0)
+    df = pd.DataFrame(
+        {
+            "id": range(n),
+            "score": [random.uniform(-1, 5) for i in range(n)],
+            "amt": random.choices(range(1000), k=n),
+            "cat": random.choices(["test", "train"], k=n),
+            "dte": [
+                datetime.date.fromisoformat(i)
+                for i in random.choices(["2022-01-01", "2022-02-02", "2022-03-03"], k=n)
+            ],
+            "time": [
+                datetime.datetime.fromisoformat(i)
+                for i in random.choices(
+                    [
+                        "2022-01-01 00:19:02.011135",
+                        "2022-02-02 23:00:00.000000",
+                        "2022-03-03 10:19:35.071235",
+                    ],
+                    k=n,
+                )
+            ],
+        }
+    )
+
+    for col in ["score", "cat", "dte", "time"]:
+        df.loc[random.choices(range(n), k=int(n / 20)), col] = None
+
+    return df
+
+
+def _parse_sch_tbl_nme(sch_tbl_nme):
+    db = dwopt.dbo._Db
+    return db._parse_sch_tbl_nme(db, sch_tbl_nme)
+
+
+def _make_pg_tbl(df, eng, sch_tbl_nme):
+    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
+    meta = alc.MetaData()
+    test_tbl = alc.Table(
+        tbl_nme,
+        meta,
+        alc.Column("id", alc.dialects.postgresql.BIGINT, primary_key=True),
+        alc.Column("score", alc.Float(8)),
+        alc.Column("amt", alc.dialects.postgresql.BIGINT),
+        alc.Column("cat", alc.String(20)),
+        alc.Column("dte", alc.Date),
+        alc.Column("time", alc.DateTime),
+        schema=sch,
+    )
+    with eng.begin() as conn:
+        test_tbl.drop(conn, checkfirst=True)
+    meta.create_all(eng)
+    with eng.begin() as conn:
+        conn.execute(
+            test_tbl.insert(),
+            df.assign(
+                time=lambda x: x.time.astype(object).where(~x.time.isna(), None)
+            ).to_dict("records"),
+        )
+
+
+def _make_lt_tbl(df, eng, sch_tbl_nme):
+    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
+    meta = alc.MetaData()
+    test_tbl = alc.Table(
+        tbl_nme,
+        meta,
+        alc.Column("id", alc.Integer, primary_key=True),
+        alc.Column("score", alc.REAL),
+        alc.Column("amt", alc.Integer),
+        alc.Column("cat", alc.String),
+        alc.Column("dte", alc.String),
+        alc.Column("time", alc.String),
+        schema=sch,
+    )
+    with eng.begin() as conn:
+        test_tbl.drop(conn, checkfirst=True)
+    meta.create_all(eng)
+    with eng.begin() as conn:
+        conn.execute(
+            test_tbl.insert(),
+            df.assign(
+                time=lambda x: x.time.astype(str).where(~x.time.isna(), None)
+            ).to_dict("records"),
+        )
+
+
+def _make_oc_tbl(df, eng, sch_tbl_nme):
+    _, sch, tbl_nme = _parse_sch_tbl_nme(sch_tbl_nme)
+    meta = alc.MetaData()
+    test_tbl = alc.Table(
+        tbl_nme,
+        meta,
+        alc.Column("id", alc.dialects.oracle.NUMBER, primary_key=True),
+        alc.Column("score", alc.Float),
+        alc.Column("amt", alc.dialects.oracle.NUMBER),
+        alc.Column("cat", alc.String(20)),
+        alc.Column("dte", alc.Date),
+        alc.Column("time", alc.Date),
+        schema=sch,
+    )
+    with eng.begin() as conn:
+        test_tbl.drop(conn, checkfirst=True)
+    meta.create_all(eng)
+    with eng.begin() as conn:
+        conn.execute(
+            test_tbl.insert(),
+            df.assign(
+                score=lambda x: x.score.astype(object).where(~x.score.isna(), None),
+                time=lambda x: x.time.astype(object).where(~x.time.isna(), None),
+            ).to_dict("records"),
+        )
+
+
+def make_test_tbl(db, sch_tbl_nme="test", n=10000):
+    """Make or remake a test table on database.
+
+    Uses Sqlalchemy toolkits for table drop, creation, insertion.
+
+    Parameters
+    ------------
+    db: dwopt.dbo._Db, or str
+        Dwopt database operator object. Or one of ``'pg'``, ``'lt'``, and ``'oc'``,
+        indicating usage of pre-defined testing database engines.
+    sch_tbl_nme: str
+        Table name in form ``my_schema1.my_table1`` or ``my_table1``.
+    n: int
+        Number of records.
+
+    Returns
+    ----------
+    (dwopt.dbo._Db, pandas.DataFrame):
+        Tuple of database operator used, and the test dataframe.
+
+    Notes
+    ------
+
+    **Table specifications**
+
+    ====== ============== ============== ==== ===================
+    Column Column type    Object type    None Example
+    ====== ============== ============== ==== ===================
+    id     int64          int64               0
+    score  float64        float64        NaN  4.066531
+    amt    int64          int64               867
+    cat    object         str            None train
+    dte    object         datetime.date  None 2022-03-03
+    time   datetime64[ns] datetime64[ns] NaT  2022-02-02 23:00:00
+    ====== ============== ============== ==== ===================
+
+    **Test database table specifications**
+
+    ====== =========== ======= ============
+    Column Postgre     Sqlite  Oracle
+    ====== =========== ======= ============
+    id     bigint      integer number
+    score  float8      real    float
+    amt    bigint      integer number
+    cat    varchar(20) text    varchar2(20)
+    dte    date        text    date
+    time   timestamp   text    date
+    ====== =========== ======= ============
+
+    These datatypes are implemented via closest
+    `Sqlalchemy datatypes <https://docs.sqlalchemy.org/en/14/core/type_basics.html>`_.
+
+    The ``id`` column is made primary key in the test database tables.
+
+    *Floating point types*
+
+    The ``score`` column's ``NaN`` objects are converted into ``None`` before insertion
+    for oracle.
+
+    *Datetime types*
+
+    The ``time`` column's ``NaT`` objects are converted into ``None`` before insertion
+    for Postgre and Oracle.
+    The ``time`` column are converted into str and None before insertion for Sqlite.
+
+    **Pre-defined testing database engines**
+
+    * ``pg``: ``postgresql://dwopt_tester:1234@localhost/dwopt_test``
+    * ``lt``: ``sqlite://``
+    * ``oc``: ``oracle://dwopt_test:1234@localhost:1521/?service_name=XEPDB1
+      &encoding=UTF-8&nencoding=UTF-8``.
+
+    **Install testing databases**
+
+    *Postgre*
+
+    * Install from
+      `postgresql windows <https://www.postgresql.org/download/windows/>`_.
+    * Add postgres bin directory to path.
+    * Run commands:
+
+      .. code-block:: console
+
+        psql -U postgres
+        CREATE DATABASE dwopt_test;
+        CREATE USER dwopt_tester WITH PASSWORD '1234';
+        GRANT ALL PRIVILEGES ON DATABASE dwopt_test to dwopt_tester;
+        ALTER DATABASE dwopt_test OWNER TO dwopt_tester;
+
+    *Postgre on linux*
+
+    .. code-block:: console
+
+        sudo su postgres
+        psql
+        CREATE DATABASE dwopt_test;
+        CREATE USER dwopt_tester WITH PASSWORD '1234';
+        GRANT ALL PRIVILEGES ON DATABASE dwopt_test to dwopt_tester;
+        ALTER DATABASE dwopt_test OWNER TO dwopt_tester;
+
+    *Oracle*
+
+    * Install from
+      `oracle xe <https://www.oracle.com/database/technologies/xe-downloads.html>`_.
+    * Set ORACLE_HOME, ORACLE_SID environment variable, and path based on the
+      `oracle configuration <https://docs.oracle.com/database/121/ADMQS/
+      GUID-EC18C4A6-3BA5-4C14-9D76-B0DD62FEFFF2.htm#ADMQS12369>`_.
+    * Run commands:
+
+      .. code-block:: console
+
+        sqlplus sys/{PASSWORD}@//localhost:1521/XEPDB1 as sysdba
+        create user dwopt_test identified by 1234;
+        grant create session to dwopt_test;
+        grant create table to dwopt_test;
+        grant unlimited tablespace to dwopt_test;
+
+    Examples
+    ----------
+    Make test table via provided database operator:
+
+    >>> from dwopt import lt, make_test_tbl
+    >>> _ = make_test_tbl(lt)
+    >>> lt.qry('test').len()
+    10000
+
+    Make database operator for the pre-defined test databases,
+    then make test table on it:
+
+    >>> from dwopt import make_test_tbl
+    >>> lt, df = make_test_tbl('lt', 'foo', 999)
+    >>> lt.eng
+    Engine(sqlite://)
+    >>> lt.qry('foo').len()
+    999
+    >>> len(df)
+    999
+    """
+    if isinstance(db, str):
+        if db == "pg":
+            db = dwopt.db(_TEST_PG_URL)
+        elif db == "lt":
+            db = dwopt.db(_TEST_LT_URL)
+        elif db == "oc":
+            db = dwopt.db(_TEST_OC_URL)
+        else:
+            raise ValueError("Invalid db str, use one of 'pg', 'lt', or 'oc'")
+    df = _make_test_df(n)
+    dlc = db._dialect
+    if dlc == "pg":
+        _make_pg_tbl(df, db.eng, sch_tbl_nme)
+    elif dlc == "lt":
+        _make_lt_tbl(df, db.eng, sch_tbl_nme)
+    elif dlc == "oc":
+        _make_oc_tbl(df, db.eng, sch_tbl_nme)
+    else:
+        raise ValueError(
+            "Invalid db, must be a database operator object, instances of "
+            "(dwopt.Pg, dwopt.Lt, dwopt.Oc)"
+        )
+    return db, df
```

### Comparing `dwopt-0.0.7/src/dwopt.egg-info/PKG-INFO` & `dwopt-0.0.8/src/dwopt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,579 +1,636 @@
-Metadata-Version: 2.1
-Name: dwopt
-Version: 0.0.7
-Summary: Datawarehouse operator
-Home-page: https://github.com/0xdomyz/dwopt
-Author: 0xdomyz
-Author-email: septemberwhyms@gmail.com
-Project-URL: Bug Tracker, https://github.com/0xdomyz/dwopt/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-DWOPT - Datawarehouse Operator
-==============================
-
-Getting summary statistics out of database tables is often an unstreamlined process.
-Does one read in millions of rows before doing any work on Python,
-or run sql elsewhere and use intermediate CSVs,
-or write sql strings in python scripts?
-
-The Python package **dwopt**
-provides Excel-pivot-table-like and dataframe-summary-methods-like API,
-driven by sql templates, under a flexible summary query building framework.
-
-See the Features and the Walk Through section for examples.
-
-.. end-of-readme-intro
-
-
-Installation
-------------
-
-.. code-block:: console
-
-    pip install dwopt
-
-
-Features
---------
-
-* `Run sql frictionlessly using saved credentials`_
-* `Run sql script with text replacement`_
-* `Programatically make simple sql query`_
-* `Templates: Excel-pivot-table-like API`_
-* `Templates: Dataframe-summary-methods-like API`_
-* `Templates: DDL/DML statements, metadata queries`_
-* `Standard logging with reproducible sql`_
-
-
-Walk Through
-------------
-
-Run sql frictionlessly using saved credentials
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
-.. |dwopt.db| replace:: ``dwopt.db``
-.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
-.. |dwopt.save_url| replace:: ``dwopt.save_url``
-.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
-
-On import, the package gives ready-to-be-used `database operator objects`_
-with default credentials, which could be saved prior by user to
-the system keyring using the |dwopt.save_url|_ function.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.run('select count(1) from iris')
-       count
-    0    150
-
-This enable quick analysis from any Python/Console window:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.qry('iris').valc('species', 'avg(petal_length)')
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, use the database operator object factory function |dwopt.db|_
-and the database engine url to access database.
-
-.. code-block:: python
-
-    from dwopt import db
-    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
-    d.mtcars()
-    d.run('select count(1) n from mtcars')
-        n
-    0  32
-
-Supports:
-
-* Python 3.9, 3.10, 3.11.
-* Windows 10: Sqlite, Postgre, Oracle.
-* Linux: Sqlite, Postgre.
-
-See `Testing`_ section for package version tested.
-
-Run sql script with text replacement
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |run| replace:: ``run``
-.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
-
-Use the database operator object's
-|run|_ method to run sql script file.
-One could then replace ``:`` marked parameters via mappings supplied to the method.
-
-.. code-block:: python
-
-    from dwopt import pg, make_test_tbl
-    _ = make_test_tbl(pg)
-    pg.run(pth = "E:/projects/my_sql_script.sql",
-        my_run_dte = '2022-03-03',
-        my_label = '20220303',
-        threshold = 5)
-       count
-    0    137
-
-Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
-
-.. code-block:: sql
-
-    drop table if exists monthly_extract_:my_label;
-
-    create table monthly_extract_:my_label as
-    select * from test
-    where
-        dte = to_date(':my_run_dte','YYYY-MM-DD')
-        and score > :threshold;
-
-    select count(1) from monthly_extract_:my_label;
-
-
-Programatically make simple sql query
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
-.. |qry| replace:: ``qry``
-.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
-.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
-.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
-
-The database operator object's |qry|_ method returns the `query object`_.
-Use it's `list of clause methods`_ to make a simple sql query.
-
-This is not faster than just writing the sql,
-main usage is to provide flexibility to the `summary query building framework`_.
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.mtcars()
-    sql = "select cyl from mtcars group by cyl having count(1) > 10"
-    q = (
-        lt.qry('mtcars a')
-        .select('a.cyl, count(1) n, avg(a.mpg)')
-        .case('cat', "a.cyl = 8 then 1", els=0)
-        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
-        .group_by('a.cyl')
-        .having('count(1) > 10')
-        .order_by('n desc')
-    )
-    q.run()
-       cyl   n  avg(a.mpg)  cat
-    0    8  14   15.100000    1
-    1    4  11   26.663636    0
-
-.. code-block:: sql
-
-    q.print()
-    select a.cyl, count(1) n, avg(a.mpg)
-        ,case when a.cyl = 8 then 1 else 0 end as cat
-    from mtcars a
-    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
-        on a.cyl = b.cyl
-    group by a.cyl
-    having count(1) > 10
-    order by n desc
-
-
-Templates: Excel-pivot-table-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |valc| replace:: ``valc``
-.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
-
-.. |pivot| replace:: ``pivot``
-.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
-
-Use the `query object`_ and it's |valc|_ method to make and run
-a value counts summary query with custom groups and calcs,
-on top of arbituary sub-query, as part of the `summary query building framework`_.
-
-Then call the result dataframe's |pivot|_ method to finalize the pivot table.
-
-.. code-block:: python
-
-    from dwopt import lt, make_test_tbl
-    _ = make_test_tbl(lt)
-    (
-        lt.qry('test')
-        .where('score>0.5', 'dte is not null', 'cat is not null')
-        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
-        .pivot('dte', 'cat')
-    )
-
-Result:
-
-==========  =====  =====  ========  ========  ======  ======
-cat           n           avgscore             total
-----------  -----  -----  --------  --------  ------  ------
-dte         test   train    test     train     test   train 
-==========  =====  =====  ========  ========  ======  ======
-2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
-2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
-2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
-==========  =====  =====  ========  ========  ======  ======
-
-The final query used can be invoked by the |valc|_ method, or logged via standard
-logging.
-
-.. code-block:: sql
-
-    with x as (
-        select * from test
-        where score>0.5
-            and dte is not null
-            and cat is not null
-    )
-    select
-        dte,cat
-        ,count(1) n
-        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
-    from x
-    group by dte,cat
-    order by n desc
-
-
-Templates: Dataframe-summary-methods-like API
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
-
-Use the `query object`_ and it's `list of summary methods`_ to make and run
-summary queries on top of arbituary sub-query,
-as part of the `summary query building framework`_:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    q = pg.qry('iris a').select('a.*').case('cat',
-        "petal_length > 5             then '5+'",
-        "petal_length between 2 and 5 then '2-5'",
-        "petal_length < 2             then '-2'",
-    )
-
-    #Column names:
-    q.cols()
-    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
-
-    #Number of distinct combination:
-    q.dist(['species', 'petal_length'])
-    count    48
-    Name: 0, dtype: int64
-
-    #Head:
-    q.head()
-       sepal_length  sepal_width  petal_length  petal_width species cat
-    0           5.1          3.5           1.4          0.2  setosa  -2
-    1           4.9          3.0           1.4          0.2  setosa  -2
-    2           4.7          3.2           1.3          0.2  setosa  -2
-    3           4.6          3.1           1.5          0.2  setosa  -2
-    4           5.0          3.6           1.4          0.2  setosa  -2
-
-    #Length:
-    q.len()
-    150
-
-    #Min and max value:
-    q.mimx('petal_length')
-    max    6.9
-    min    1.0
-    Name: 0, dtype: float64
-
-    #Top record:
-    q.top()
-    sepal_length       5.1
-    sepal_width        3.5
-    petal_length       1.4
-    petal_width        0.2
-    species         setosa
-    cat                 -2
-    Name: 0, dtype: object
-
-    #Value count followed by pivot:
-    q.valc('species, cat').pivot('species','cat','n')
-    cat        -2   2-5    5+
-    species
-    rginica   NaN   9.0  41.0
-    setosa   50.0   NaN   NaN
-    sicolor   NaN  49.0   1.0
-
-.. code-block:: sql
-
-    #--All summary methods support output by printing or str:
-    q.valc('species, cat', out=1)
-    with x as (
-        select a.*
-            ,case
-                when petal_length > 5             then '5+'
-                when petal_length between 2 and 5 then '2-5'
-                when petal_length < 2             then '-2'
-                else NULL
-            end as cat
-        from iris a
-    )
-    select
-        species, cat
-        ,count(1) n
-    from x
-    group by species, cat
-    order by n desc
-
-Templates: DDL/DML statements, metadata queries
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
-.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
-
-Use the `list of operation methods`_ to make and run some
-DDL/DML statements with convenient or enhanced functionalities:
-
-.. code-block:: python
-
-    import pandas as pd
-    from dwopt import lt
-    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
-    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
-    lt.drop('test')
-    lt.create('test', col1='int', col2='text')
-    lt.write(tbl, 'test')
-    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
-    lt.run("select * from test")
-       col1 col2
-    0     1    a
-    1     2    b
-    2     3    c
-
-.. code-block:: python
-
-    lt.drop('test')
-    lt.cwrite(tbl, 'test')
-    lt.qry('test').run()
-       col1 col2
-    0     1    a
-    1     2    b
-
-
-Use the `list of metadata methods`_ to make and run some useful metadata queries:
-
-.. code-block:: python
-
-    from dwopt import pg
-    pg.iris()
-    pg.table_cols('public.iris')
-        column_name          data_type
-    0  sepal_length               real
-    1   sepal_width               real
-    2  petal_length               real
-    3   petal_width               real
-    4       species  character varying
-
-.. code-block:: python
-
-    from dwopt import lt
-    lt.iris()
-    lt.mtcars()
-    lt.list_tables().iloc[:,:-1]
-        type    name tbl_name  rootpage
-    0  table    iris     iris         2
-    1  table  mtcars   mtcars         5
-
-
-Standard logging with reproducible sql
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |INFO| replace:: ``INFO``
-.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
-
-Many of the package's methods are wired through the standard
-`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
-package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
-The relevant logger object has standard naming and is called ``dwopt.dbo``.
-
-Example configuration to show logs in console:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(level = logging.INFO)
-
-    from dwopt import lt
-    lt.iris(q=1).valc('species', 'avg(petal_length)')
-
-.. code-block:: text
-
-    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:creating table via sqlalchemy:
-    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
-    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
-    INFO:dwopt.dbo:args len=150, e.g.
-    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
-    INFO:dwopt.dbo:done
-    INFO:dwopt.dbo:running:
-    with x as (
-        select * from iris
-    )
-    select
-        species
-        ,count(1) n
-        ,avg(petal_length)
-    from x
-    group by species
-    order by n desc
-    INFO:dwopt.dbo:done
-       species   n  avg(petal_length)
-    0  sicolor  50              4.260
-    1   setosa  50              1.462
-    2  rginica  50              5.552
-
-Alternatively, to avoid logging info messages from other packages:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Example configuration to print on console and store on file with timestamps:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig(
-        format = "%(asctime)s [%(levelname)s] %(message)s"
-        ,handlers=[
-            logging.FileHandler("E:/projects/logs.log"),
-            logging.StreamHandler()
-        ]
-    )
-    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
-
-Sqlalchemy logger can also be used to obtain even more details:
-
-.. code-block:: python
-
-    import logging
-    logging.basicConfig()
-    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
-
-
-Development
----------------
-
-Installation
-^^^^^^^^^^^^^^^
-
-Testing, documentation building package:
-
-.. code-block:: console
-
-    #testing
-    python -m pip install pytest black flake8 tox
-    
-    #doco and packaging
-    python -m pip install sphinx sphinx_rtd_theme build twine
-    
-    #depend
-    python -m pip install -U sqlalchemy psycopg2 cx_Oracle pandas keyring
-    
-    #package
-    python -m pip install -e .
-
-Testing
-^^^^^^^^^^^^
-
-Test:
-
-.. code-block:: console
-
-    python -m tox
-
-.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
-.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
-
-Testing for specific databases.
-Set up environment based on |dwopt.make_test_tbl|_ function notes.
-
-.. code-block:: console
-
-    python -m pytest
-    python -m pytest --db=pg
-    python -m pytest --db=oc
-
-Test code styles:
-
-.. code-block:: console
-
-    flake8 src/dwopt
-
-Package versions tested are::
-
-    Name: SQLAlchemy
-    Version: 2.0.7
-    ---
-    Name: psycopg2
-    Version: 2.9.5
-    ---
-    Name: cx-Oracle
-    Version: 8.3.0
-    ---
-    Name: pandas
-    Version: 1.5.3
-    ---
-    Name: keyring
-    Version: 23.13.1
-
-Documentation
-^^^^^^^^^^^^^^^^^
-
-Build document:
-
-.. code-block:: console
-
-    cd docs
-    make html
-
-Test examples across docs:
-
-.. code-block:: console
-
-    cd docs
-    make doctest
-
-Future
-^^^^^^^^^
-
-* For text replacement directives, use
-  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
-* Add more summary, DML/DDL, metadata templates.
-
-.. end-of-readme-usage
-
-
-Documentation
--------------
-
-* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
+Metadata-Version: 2.1
+Name: dwopt
+Version: 0.0.8
+Summary: SQL query abstraction library
+Home-page: https://github.com/0xdomyz/dwopt
+Author: 0xdomyz
+Author-email: septemberwhyms@gmail.com
+Project-URL: Bug Tracker, https://github.com/0xdomyz/dwopt/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+DWOPT - SQL query abstraction library
+========================================
+
+Getting summary statistics out of database tables is often an unstreamlined process.
+Does one read in millions of rows before doing any work on Python,
+or run SQL elsewhere and use intermediate CSVs,
+or write sql strings in python scripts?
+
+The Python package **dwopt** (Datawarehouse Operator)
+uses classes with a collection of sql templates to dynamically build and run queries,
+under a flexible summary query building framework.
+
+Specifically, it features Excel-pivot-table-like API,
+a collection of dataframe-summary-methods-like API,
+and a collection of DDL/DML statements, metadata query wrappers.
+
+Supports:
+
+* Python 3.10, 3.11.
+* Windows 10: Sqlite, Postgres, Oracle.
+* Linux: Sqlite, Postgres.
+
+See the Features and the Walk Through section for examples.
+
+.. end-of-readme-intro
+
+
+Installation
+------------
+
+.. code-block:: console
+
+    pip install dwopt
+
+Install the database drivers for the database engines you want to use.
+
+.. code-block:: console
+
+    pip install psycopg2 # postgres
+    pip install psycopg2-binary # in case can't build psycopg2
+    
+    pip install oracledb # oracle
+
+Features
+--------
+
+* `Run sql frictionlessly using saved credentials`_
+* `Run sql script with text replacement`_
+* `Programatically make simple sql query`_
+* `Templates: Excel-pivot-table-like API`_
+* `Templates: Dataframe-summary-methods-like API`_
+* `Templates: DDL/DML statements, metadata queries`_
+* `Standard logging with reproducible sql`_
+
+
+Walk Through
+------------
+
+Run sql frictionlessly using saved credentials
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _database operator objects: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db
+.. |dwopt.db| replace:: ``dwopt.db``
+.. _dwopt.db: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.db
+.. |dwopt.save_url| replace:: ``dwopt.save_url``
+.. _dwopt.save_url: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.save_url
+
+On import, the package gives ready-to-be-used `database operator objects`_
+with default credentials, which could be saved prior by user to
+the system keyring using the |dwopt.save_url|_ function.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.run('select count(1) from iris')
+       count
+    0    150
+
+This enable quick analysis from any Python/Console window:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.qry('iris').valc('species', 'avg(petal_length)')
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, use the database operator object factory function |dwopt.db|_
+and the database engine url to access database.
+
+.. code-block:: python
+
+    from dwopt import db
+    d = db("postgresql://dwopt_tester:1234@localhost/dwopt_test")
+    d.mtcars()
+    d.run('select count(1) n from mtcars')
+        n
+    0  32
+
+Allows for thick mode connection to Oracle database:
+
+.. code-block:: python
+
+    from dwopt import db
+    url = """oracle+oracledb://dwopt_test:1234@localhost:1521/?service_name=XEPDB1 
+    &encoding=UTF-8&nencoding=UTF-8"""
+    lib_dir = "C:/app/{user_name}/product/21c/dbhomeXE/bin"
+    o = db(url, thick_mode={"lib_dir": lib_dir})
+    o.run("select * from dual")
+      dummy
+    0     X
+
+See `Testing`_ section for package version tested.
+
+Run sql script with text replacement
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |run| replace:: ``run``
+.. _run: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.dbo._Db.run
+
+Use the database operator object's
+|run|_ method to run sql script file.
+One could then replace ``:`` marked parameters via mappings supplied to the method.
+
+Colon syntax is to be deprecated.
+A future version will use jinja2 syntax across the board.
+
+.. code-block:: python
+
+    from dwopt import pg, make_test_tbl
+    _ = make_test_tbl(pg)
+    pg.run(pth = "E:/projects/my_sql_script.sql",
+        my_run_dte = '2022-03-03',
+        my_label = '20220303',
+        threshold = 5)
+       count
+    0    137
+
+Above runs the sql stored on ``E:/projects/my_sql_script.sql`` as below:
+
+.. code-block:: sql
+
+    drop table if exists monthly_extract_:my_label;
+
+    create table monthly_extract_:my_label as
+    select * from test
+    where
+        dte = to_date(':my_run_dte','YYYY-MM-DD')
+        and score > :threshold;
+
+    select count(1) from monthly_extract_:my_label;
+
+
+Programatically make simple sql query
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of clause methods: https://dwopt.readthedocs.io/en/stable/api.html#clause-methods
+.. |qry| replace:: ``qry``
+.. _qry: https://dwopt.readthedocs.io/en/stable/dbo.html#dwopt.db._Db.qry
+.. _summary query building framework: https://dwopt.readthedocs.io/en/stable/qry.html#the-summary-query-building-framework
+.. _query object: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry
+
+The database operator object's |qry|_ method returns the `query object`_.
+Use it's `list of clause methods`_ to make a simple sql query.
+
+This is not faster than just writing the sql,
+main usage is to provide flexibility to the `summary query building framework`_.
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.mtcars()
+    sql = "select cyl from mtcars group by cyl having count(1) > 10"
+    q = (
+        lt.qry('mtcars a')
+        .select('a.cyl, count(1) n, avg(a.mpg)')
+        .case('cat', "a.cyl = 8 then 1", els=0)
+        .join(f'({sql}) b', 'a.cyl = b.cyl', how='inner')
+        .group_by('a.cyl')
+        .having('count(1) > 10')
+        .order_by('n desc')
+    )
+    q.run()
+       cyl   n  avg(a.mpg)  cat
+    0    8  14   15.100000    1
+    1    4  11   26.663636    0
+
+.. code-block:: sql
+
+    q.print()
+    select a.cyl, count(1) n, avg(a.mpg)
+        ,case when a.cyl = 8 then 1 else 0 end as cat
+    from mtcars a
+    inner join (select cyl from mtcars group by cyl having count(1) > 10) b
+        on a.cyl = b.cyl
+    group by a.cyl
+    having count(1) > 10
+    order by n desc
+
+
+Templates: Excel-pivot-table-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |valc| replace:: ``valc``
+.. _valc: https://dwopt.readthedocs.io/en/stable/qry.html#dwopt._qry._Qry.valc
+
+.. |pivot| replace:: ``pivot``
+.. _pivot: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html
+
+Use the `query object`_ and it's |valc|_ method to make and run
+a value counts summary query with custom groups and calcs,
+on top of arbituary sub-query, as part of the `summary query building framework`_.
+
+Then call the result dataframe's |pivot|_ method to finalize the pivot table.
+
+.. code-block:: python
+
+    from dwopt import lt, make_test_tbl
+    _ = make_test_tbl(lt)
+    (
+        lt.qry('test')
+        .where('score>0.5', 'dte is not null', 'cat is not null')
+        .valc('dte,cat', 'avg(score) avgscore, round(sum(amt)/1e3,2) total')
+        .pivot('dte', 'cat')
+    )
+
+Result:
+
+==========  =====  =====  ========  ========  ======  ======
+cat           n           avgscore             total
+----------  -----  -----  --------  --------  ------  ------
+dte         test   train    test     train     test   train 
+==========  =====  =====  ========  ========  ======  ======
+2022-01-01  1140   1051   2.736275  2.800106  565.67  530.09
+2022-02-02  1077   1100   2.759061  2.748898  536.68  544.10
+2022-03-03  1037   1072   2.728527  2.743825  521.54  528.85
+==========  =====  =====  ========  ========  ======  ======
+
+The final query used can be invoked by the |valc|_ method, or logged via standard
+logging.
+
+.. code-block:: sql
+
+    with x as (
+        select * from test
+        where score>0.5
+            and dte is not null
+            and cat is not null
+    )
+    select
+        dte,cat
+        ,count(1) n
+        ,avg(score) avgscore, round(sum(amt)/1e3,2) total
+    from x
+    group by dte,cat
+    order by n desc
+
+
+Templates: Dataframe-summary-methods-like API
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of summary methods: https://dwopt.readthedocs.io/en/stable/api.html#summary-methods
+
+Use the `query object`_ and it's `list of summary methods`_ to make and run
+summary queries on top of arbituary sub-query,
+as part of the `summary query building framework`_:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    q = pg.qry('iris a').select('a.*').case('cat',
+        "petal_length > 5             then '5+'",
+        "petal_length between 2 and 5 then '2-5'",
+        "petal_length < 2             then '-2'",
+    )
+
+    #Column names:
+    q.cols()
+    ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species', 'cat']
+
+    #Number of distinct combination:
+    q.dist(['species', 'petal_length'])
+    count    48
+    Name: 0, dtype: int64
+
+    #Head:
+    q.head()
+       sepal_length  sepal_width  petal_length  petal_width species cat
+    0           5.1          3.5           1.4          0.2  setosa  -2
+    1           4.9          3.0           1.4          0.2  setosa  -2
+    2           4.7          3.2           1.3          0.2  setosa  -2
+    3           4.6          3.1           1.5          0.2  setosa  -2
+    4           5.0          3.6           1.4          0.2  setosa  -2
+
+    #Length:
+    q.len()
+    150
+
+    #Min and max value:
+    q.mimx('petal_length')
+    max    6.9
+    min    1.0
+    Name: 0, dtype: float64
+
+    #Top record:
+    q.top()
+    sepal_length       5.1
+    sepal_width        3.5
+    petal_length       1.4
+    petal_width        0.2
+    species         setosa
+    cat                 -2
+    Name: 0, dtype: object
+
+    #Value count followed by pivot:
+    q.valc('species, cat').pivot('species','cat','n')
+    cat        -2   2-5    5+
+    species
+    rginica   NaN   9.0  41.0
+    setosa   50.0   NaN   NaN
+    sicolor   NaN  49.0   1.0
+
+.. code-block:: sql
+
+    #--All summary methods support output by printing or str:
+    q.valc('species, cat', out=1)
+    with x as (
+        select a.*
+            ,case
+                when petal_length > 5             then '5+'
+                when petal_length between 2 and 5 then '2-5'
+                when petal_length < 2             then '-2'
+                else NULL
+            end as cat
+        from iris a
+    )
+    select
+        species, cat
+        ,count(1) n
+    from x
+    group by species, cat
+    order by n desc
+
+Templates: DDL/DML statements, metadata queries
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. _list of metadata methods: https://dwopt.readthedocs.io/en/stable/api.html#metadata-methods
+.. _list of operation methods: https://dwopt.readthedocs.io/en/stable/api.html#operation-methods
+
+Use the `list of operation methods`_ to make and run some
+DDL/DML statements with convenient or enhanced functionalities:
+
+.. code-block:: python
+
+    import pandas as pd
+    from dwopt import lt
+    tbl = pd.DataFrame({'col1': [1, 2], 'col2': ['a', 'b']})
+    tbl2 = pd.DataFrame({'col1': [1, 3], 'col2': ['a', 'c']})
+    lt.drop('test')
+    lt.create('test', col1='int', col2='text')
+    lt.write(tbl, 'test')
+    lt.write_nodup(tbl2, 'test', ['col1'], "col1 < 4")
+    lt.run("select * from test")
+       col1 col2
+    0     1    a
+    1     2    b
+    2     3    c
+
+.. code-block:: python
+
+    lt.drop('test')
+    lt.cwrite(tbl, 'test')
+    lt.qry('test').run()
+       col1 col2
+    0     1    a
+    1     2    b
+
+
+Use the `list of metadata methods`_ to make and run some useful metadata queries:
+
+.. code-block:: python
+
+    from dwopt import pg
+    pg.iris()
+    pg.table_cols('public.iris')
+        column_name          data_type
+    0  sepal_length               real
+    1   sepal_width               real
+    2  petal_length               real
+    3   petal_width               real
+    4       species  character varying
+
+.. code-block:: python
+
+    from dwopt import lt
+    lt.iris()
+    lt.mtcars()
+    lt.list_tables().iloc[:,:-1]
+        type    name tbl_name  rootpage
+    0  table    iris     iris         2
+    1  table  mtcars   mtcars         5
+
+
+Standard logging with reproducible sql
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |INFO| replace:: ``INFO``
+.. _INFO: https://docs.python.org/3/howto/logging.html#when-to-use-logging
+
+Many of the package's methods are wired through the standard
+`logging <https://docs.python.org/3/library/logging.html#module-logging>`_
+package. In particular, the |run|_ method emits sql used as |INFO|_ level message.
+The relevant logger object has standard naming and is called ``dwopt.dbo``.
+
+Example configuration to show logs in console:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(level = logging.INFO)
+
+    from dwopt import lt
+    lt.iris(q=1).valc('species', 'avg(petal_length)')
+
+.. code-block:: text
+
+    INFO:dwopt.dbo:dropping table via sqlalchemy: iris
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:creating table via sqlalchemy:
+    INFO:dwopt.dbo:('sepal_length', Column('sepal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('sepal_width', Column('sepal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_length', Column('petal_length', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('petal_width', Column('petal_width', REAL(), table=<iris>))
+    INFO:dwopt.dbo:('species', Column('species', String(), table=<iris>))
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    INSERT INTO iris (sepal_length, sepal_width, petal_length, petal_width, species) VALUES (:sepal_length, :sepal_width, :petal_length, :petal_width, :species)
+    INFO:dwopt.dbo:args len=150, e.g.
+    {'sepal_length': 5.1, 'sepal_width': 3.5, 'petal_length': 1.4, 'petal_width': 0.2, 'species': 'setosa'}
+    INFO:dwopt.dbo:done
+    INFO:dwopt.dbo:running:
+    with x as (
+        select * from iris
+    )
+    select
+        species
+        ,count(1) n
+        ,avg(petal_length)
+    from x
+    group by species
+    order by n desc
+    INFO:dwopt.dbo:done
+       species   n  avg(petal_length)
+    0  sicolor  50              4.260
+    1   setosa  50              1.462
+    2  rginica  50              5.552
+
+Alternatively, to avoid logging info messages from other packages:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Example configuration to print on console and store on file with timestamps:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig(
+        format = "%(asctime)s [%(levelname)s] %(message)s"
+        ,handlers=[
+            logging.FileHandler("E:/projects/logs.log"),
+            logging.StreamHandler()
+        ]
+    )
+    logging.getLogger('dwopt.dbo').setLevel(logging.INFO)
+
+Debug logging:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('dwopt').setLevel(logging.DEBUG)
+
+Sqlalchemy logger can also be used to obtain even more details:
+
+.. code-block:: python
+
+    import logging
+    logging.basicConfig()
+    logging.getLogger('sqlalchemy.engine').setLevel(logging.INFO)
+
+
+Development
+---------------
+
+Installation
+^^^^^^^^^^^^^^^
+
+Testing, documentation building package:
+
+.. code-block:: console
+
+    #venv on linux
+    sudo apt-get install python3-venv
+    python3.11 -m venv dwopt_dev
+    source dwopt_dev/bin/activate
+    deactivate
+
+    #testing
+    python -m pip install pytest black flake8 tox
+    
+    #doco and packaging
+    python -m pip install sphinx sphinx_rtd_theme build twine wheel
+    
+    #depend
+    python -m pip install -U sqlalchemy pandas keyring
+    python -m pip install -U keyrings.alt
+    python -m pip install -U psycopg2
+    python -m pip install -U oracledb
+    
+    #consider
+    python -m pip install -U psycopg2-binary
+    python -m pip install -U cx_Oracle
+    
+    #package
+    python -m pip install -e .
+
+Testing
+^^^^^^^^^^^^
+
+Test:
+
+.. code-block:: console
+
+    python -m tox
+
+.. |dwopt.make_test_tbl| replace:: ``dwopt.make_test_tbl``
+.. _dwopt.make_test_tbl: https://dwopt.readthedocs.io/en/stable/set_up.html#dwopt.make_test_tbl
+
+Testing for specific databases.
+Set up environment based on |dwopt.make_test_tbl|_ function notes.
+
+.. code-block:: console
+
+    python -m pytest
+    python -m pytest --db=pg
+    python -m pytest --db=oc
+
+Test code styles:
+
+.. code-block:: console
+
+    flake8 src/dwopt
+
+Databases used for testings are::
+
+    Postgres 15
+    Oracle express 21c
+
+Package versions tested are::
+
+    Name: keyring
+    Version: 24.2.0
+    ---
+    Name: keyrings.alt
+    Version: 5.0.0
+    ---
+    Name: oracledb
+    Version: 1.3.2
+    ---
+    Name: pandas
+    Version: 2.0.3
+    ---
+    Name: psycopg2-binary
+    Version: 2.9.6
+    ---
+    Name: SQLAlchemy
+    Version: 2.0.19
+
+
+Documentation
+^^^^^^^^^^^^^^^^^
+
+Build document:
+
+.. code-block:: console
+
+    cd docs
+    make html
+
+Test examples across docs:
+
+.. code-block:: console
+
+    cd docs
+    make doctest
+
+Future
+^^^^^^^^^
+
+* For text replacement directives, use
+  `jinja2 <https://jinja2docs.readthedocs.io/en/stable/>`_ syntax.
+* Add more summary, DML/DDL, metadata templates.
+
+.. end-of-readme-usage
+
+
+Documentation
+-------------
+
+* `API <https://dwopt.readthedocs.io/en/stable/api.html>`_
```

### Comparing `dwopt-0.0.7/tests/test_db_meta.py` & `dwopt-0.0.8/tests/test_db_meta.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from pandas.testing import assert_frame_equal
-
-from dwopt import Lt, Oc, Pg, make_eng
-from dwopt._qry import _Qry
-from dwopt.testing import _TEST_LT_URL, _TEST_OC_URL, _TEST_PG_URL
-
-
-def test_db_meta_init(test_tbl):
-    db, _ = test_tbl
-    if isinstance(db, Pg):
-        Pg(_TEST_PG_URL).list_tables()
-        Pg(make_eng(_TEST_PG_URL)).list_tables()
-    elif isinstance(db, Lt):
-        Lt(_TEST_LT_URL).list_tables()
-        Lt(make_eng(_TEST_LT_URL)).list_tables()
-    elif isinstance(db, Oc):
-        Oc(_TEST_OC_URL).qry("dual").run()
-        Oc(make_eng(_TEST_OC_URL)).qry("dual").run()
-    else:
-        raise ValueError("Invalid db")
-
-
-def test_db_meta_qry(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test")
-    exp = _Qry
-    assert isinstance(act, exp)
-
-
-def test_db_meta_list_tables(test_tbl):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        sql = """
-select
-    table_catalog,table_schema,table_name
-    ,is_insertable_into,commit_action
-from information_schema.tables
-where table_schema
-not in ('information_schema','pg_catalog')
-"""
-        act = db.list_tables()
-    elif isinstance(db, Lt):
-        sql = """
-select * from sqlite_master
-where type ='table'
-and name NOT LIKE 'sqlite_%'
-"""
-        act = db.list_tables()
-    elif isinstance(db, Oc):
-        sql = """
-select/*+PARALLEL (4)*/ owner,table_name
-    ,max(column_name),min(column_name)
-from all_tab_columns
-where owner = 'DWOPT_TEST'
-group by owner,table_name
-"""
-        act = db.list_tables("dwopt_test")
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
-
-
-def test_db_meta_table_cols(test_tbl):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        sql = """
-select column_name, data_type
-from information_schema.columns
-where table_schema = 'public'
-and table_name = 'test'
-"""
-        act = db.table_cols("public.test")
-    elif isinstance(db, Lt):
-        assert True
-        return
-    elif isinstance(db, Oc):
-        sql = """
-select/*+PARALLEL (4)*/ *
-from all_tab_columns
-where owner = 'test_schema'
-and table_name = 'test'
-"""
-        act = db.table_cols("test_schema.test")
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
-
-
-def test_db_meta_table_sizes(test_tbl):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        assert True
-        return
-    elif isinstance(db, Lt):
-        assert True
-        return
-    elif isinstance(db, Oc):
-        sql = """
-select/*+PARALLEL (4)*/
-    tablespace_name,segment_type,segment_name
-    ,sum(bytes)/1024/1024 table_size_mb
-from user_extents
-group by tablespace_name,segment_type,segment_name
-"""
-    act = db.table_sizes()
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
-
-
-def test_db_meta_list_cons(test_tbl):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        sql = """
-select * from information_schema.constraint_table_usage
-"""
-    elif isinstance(db, Lt):
-        assert True
-        return
-    elif isinstance(db, Oc):
-        assert True
-        return
-    act = db.list_cons()
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
+from pandas.testing import assert_frame_equal
+
+from dwopt import Lt, Oc, Pg, make_eng
+from dwopt._qry import _Qry
+from dwopt.testing import _TEST_LT_URL, _TEST_OC_URL, _TEST_PG_URL
+
+
+def test_db_meta_init(test_tbl):
+    db, _ = test_tbl
+    if isinstance(db, Pg):
+        Pg(_TEST_PG_URL).list_tables()
+        Pg(make_eng(_TEST_PG_URL)).list_tables()
+    elif isinstance(db, Lt):
+        Lt(_TEST_LT_URL).list_tables()
+        Lt(make_eng(_TEST_LT_URL)).list_tables()
+    elif isinstance(db, Oc):
+        Oc(_TEST_OC_URL).qry("dual").run()
+        Oc(make_eng(_TEST_OC_URL)).qry("dual").run()
+    else:
+        raise ValueError("Invalid db")
+
+
+def test_db_meta_qry(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test")
+    exp = _Qry
+    assert isinstance(act, exp)
+
+
+def test_db_meta_list_tables(test_tbl):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        sql = """
+select
+    table_catalog,table_schema,table_name
+    ,is_insertable_into,commit_action
+from information_schema.tables
+where table_schema
+not in ('information_schema','pg_catalog')
+"""
+        act = db.list_tables()
+    elif isinstance(db, Lt):
+        sql = """
+select * from sqlite_master
+where type ='table'
+and name NOT LIKE 'sqlite_%'
+"""
+        act = db.list_tables()
+    elif isinstance(db, Oc):
+        sql = """
+select/*+PARALLEL (4)*/ owner,table_name
+    ,max(column_name),min(column_name)
+from all_tab_columns
+where owner = 'DWOPT_TEST'
+group by owner,table_name
+"""
+        act = db.list_tables("dwopt_test")
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
+
+
+def test_db_meta_table_cols(test_tbl):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        sql = """
+select column_name, data_type
+from information_schema.columns
+where table_schema = 'public'
+and table_name = 'test'
+"""
+        act = db.table_cols("public.test")
+    elif isinstance(db, Lt):
+        assert True
+        return
+    elif isinstance(db, Oc):
+        sql = """
+select/*+PARALLEL (4)*/ *
+from all_tab_columns
+where owner = 'test_schema'
+and table_name = 'test'
+"""
+        act = db.table_cols("test_schema.test")
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
+
+
+def test_db_meta_table_sizes(test_tbl):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        assert True
+        return
+    elif isinstance(db, Lt):
+        assert True
+        return
+    elif isinstance(db, Oc):
+        sql = """
+select/*+PARALLEL (4)*/
+    tablespace_name,segment_type,segment_name
+    ,sum(bytes)/1024/1024 table_size_mb
+from user_extents
+group by tablespace_name,segment_type,segment_name
+"""
+    act = db.table_sizes()
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
+
+
+def test_db_meta_list_cons(test_tbl):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        sql = """
+select * from information_schema.constraint_table_usage
+"""
+    elif isinstance(db, Lt):
+        assert True
+        return
+    elif isinstance(db, Oc):
+        assert True
+        return
+    act = db.list_cons()
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
```

### Comparing `dwopt-0.0.7/tests/test_db_opt.py` & `dwopt-0.0.8/tests/test_db_opt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,227 +1,229 @@
-from pandas.testing import assert_frame_equal
-from dwopt import Pg, Lt, Oc
-import pandas as pd
-import datetime
-import pytest
-
-
-def assert_frame_equal_reset_index(a, b):
-    assert_frame_equal(a.reset_index(drop=True), b.reset_index(drop=True))
-
-
-def test_db_opt_run(test_tbl):
-    db, df = test_tbl
-
-    if isinstance(db, Lt):
-        exp = df.assign(
-            dte=lambda x: x.dte.astype(str).where(~x.dte.isna(), None),
-            time=lambda x: x.time.astype(str).where(~x.time.isna(), None),
-        ).loc[lambda x: x.id <= 9, :]
-    elif isinstance(db, Pg):
-        exp = df.loc[lambda x: x.id <= 9, :]
-    elif isinstance(db, Oc):
-        exp = df.assign(
-            dte=lambda x: x["dte"].apply(
-                lambda x: datetime.datetime.combine(x, datetime.time()) if x else None
-            ),
-            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0)),
-        ).loc[lambda x: x.id <= 9, :]
-        # import pdb;pdb.set_trace()
-    else:
-        raise ValueError
-
-    act = db.run("select * from test where id <= 9 order by id")
-    assert_frame_equal_reset_index(act, exp)
-
-    act = db.run("select * from test where id <= :id order by id", args={"id": 9})
-    assert_frame_equal_reset_index(act, exp)
-
-    act = db.run("select * from test where id <= :id order by id", mods={"id": 9})
-    assert_frame_equal_reset_index(act, exp)
-
-    act = db.run("select * from test where id <= :id order by id", id=9)
-    assert_frame_equal_reset_index(act, exp)
-
-
-def test_db_opt_create(test_tbl, test_tbl2):
-    db, df = test_tbl
-
-    if isinstance(db, Pg):
-        db.create(
-            "test2",
-            dtypes={
-                "id": "bigint primary key",
-                "score": "float8",
-                "amt": "bigint",
-                "cat": "varchar(20)",
-            },
-            dte="date",
-            time="timestamp",
-        )
-    elif isinstance(db, Lt):
-        db.create(
-            "test2",
-            dtypes={
-                "id": "integer primary key",
-                "score": "real",
-                "amt": "integer",
-                "cat": "text",
-            },
-            dte="text",
-            time="text",
-        )
-    elif isinstance(db, Oc):
-        db.create(
-            "test2",
-            dtypes={
-                "id": "number primary key",
-                "score": "float",
-                "amt": "number",
-                "cat": "varchar2(20)",
-            },
-            dte="date",
-            time="timestamp",
-        )
-    else:
-        raise ValueError
-
-    db.run("insert into test2 select * from test")
-    act = db.run("select * from test2 order by id")
-    exp = db.run("select * from test order by id")
-    assert_frame_equal_reset_index(act, exp)
-
-
-def test_db_opt_add_pkey(test_tbl, test_tbl2):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        db.run("create table test2 as select * from test")
-        db.add_pkey("test2", "id")
-    elif isinstance(db, Lt):
-        pass
-    elif isinstance(db, Oc):
-        pass
-    else:
-        raise ValueError
-
-
-def test_db_opt_create_schema(test_tbl, test_tbl2):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        try:
-            db.run("drop schema test cascade")
-        except Exception as ex:
-            if "does not exist" in str(ex):
-                pass
-            else:
-                raise (ex)
-        db.create_schema("test")
-        db.run("create table test.test (col int)")
-        db.run("drop schema test cascade")
-    elif isinstance(db, Lt):
-        pass
-    elif isinstance(db, Oc):
-        pass
-    else:
-        raise ValueError
-
-
-def test_db_opt_drop(test_tbl, test_tbl2):
-    db, df = test_tbl
-    db.run("create table test2 as select * from test")
-    db.drop("test2")
-    with pytest.raises(Exception) as e_info:
-        db.run("select count(1) from test2")
-
-
-def test_db_opt_write_nodup(test_tbl, test_tbl2):
-    db, df = test_tbl
-    db.run("create table test2 as select * from test where 1=2")
-    if isinstance(db, Pg):
-        db.write(df, "test2")
-        db.write_nodup(df, "test2", ["id"])
-        tbl = db.run("select * from test2 order by id")
-        assert_frame_equal_reset_index(tbl, df)
-    elif isinstance(db, Lt):
-        db.write(
-            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
-            "test2",
-        )
-        db.write_nodup(
-            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
-            "test2",
-            ["id"],
-        )
-        tbl = (
-            db.qry("test2")
-            .run()
-            .assign(
-                dte=lambda x: x["dte"].apply(
-                    lambda x: datetime.date.fromisoformat(x) if x else None
-                ),
-                time=lambda x: pd.to_datetime(x.time),
-            )
-        )
-        assert_frame_equal_reset_index(tbl, df)
-    elif isinstance(db, Oc):
-        db.write(
-            df,
-            "test2",
-        )
-        db.write_nodup(
-            df,
-            "test2",
-            ["id"],
-        )
-        tbl = db.run("select * from test2 order by id").assign(
-            dte=lambda x: x["dte"].apply(lambda x: x.date() if x else None)
-        )
-        df2 = df.assign(
-            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
-        )
-        assert_frame_equal_reset_index(tbl, df2)
-    else:
-        raise ValueError
-
-
-def test_db_opt_cwrite(test_tbl, test_tbl2):
-    db, df = test_tbl
-    if isinstance(db, Pg):
-        db.cwrite(df, "test2")
-        tbl = db.run("select * from test2 order by id").assign(
-            dte=lambda x: x["dte"].apply(
-                lambda x: datetime.date.fromisoformat(x) if x else None
-            )
-        )
-    elif isinstance(db, Lt):
-        db.cwrite(
-            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
-            "test2",
-        )
-        tbl = (
-            db.qry("test2")
-            .run()
-            .assign(
-                dte=lambda x: x["dte"].apply(
-                    lambda x: datetime.date.fromisoformat(x) if x else None
-                ),
-                time=lambda x: pd.to_datetime(x.time),
-            )
-        )
-    elif isinstance(db, Oc):
-        db.cwrite(
-            df,
-            "test2",
-        )
-        tbl = db.run("select * from test2 order by id").assign(
-            dte=lambda x: x["dte"].apply(
-                lambda x: datetime.datetime.strptime(x, "%d-%b-%y").date()
-                if x
-                else None
-            )
-        )
-        df = df.assign(
-            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
-        )
-    else:
-        raise ValueError
-    assert_frame_equal_reset_index(tbl, df)
+import datetime
+
+import pandas as pd
+import pytest
+from pandas.testing import assert_frame_equal
+
+from dwopt import Lt, Oc, Pg
+
+
+def assert_frame_equal_reset_index(a, b):
+    assert_frame_equal(a.reset_index(drop=True), b.reset_index(drop=True))
+
+
+def test_db_opt_run(test_tbl):
+    db, df = test_tbl
+
+    if isinstance(db, Lt):
+        exp = df.assign(
+            dte=lambda x: x.dte.astype(str).where(~x.dte.isna(), None),
+            time=lambda x: x.time.astype(str).where(~x.time.isna(), None),
+        ).loc[lambda x: x.id <= 9, :]
+    elif isinstance(db, Pg):
+        exp = df.loc[lambda x: x.id <= 9, :]
+    elif isinstance(db, Oc):
+        exp = df.assign(
+            dte=lambda x: x["dte"].apply(
+                lambda x: datetime.datetime.combine(x, datetime.time()) if x else None
+            ),
+            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0)),
+        ).loc[lambda x: x.id <= 9, :]
+        # import pdb;pdb.set_trace()
+    else:
+        raise ValueError
+
+    act = db.run("select * from test where id <= 9 order by id")
+    assert_frame_equal_reset_index(act, exp)
+
+    act = db.run("select * from test where id <= :id order by id", args={"id": 9})
+    assert_frame_equal_reset_index(act, exp)
+
+    act = db.run("select * from test where id <= :id order by id", mods={"id": 9})
+    assert_frame_equal_reset_index(act, exp)
+
+    act = db.run("select * from test where id <= :id order by id", id=9)
+    assert_frame_equal_reset_index(act, exp)
+
+
+def test_db_opt_create(test_tbl, test_tbl2):
+    db, df = test_tbl
+
+    if isinstance(db, Pg):
+        db.create(
+            "test2",
+            dtypes={
+                "id": "bigint primary key",
+                "score": "float8",
+                "amt": "bigint",
+                "cat": "varchar(20)",
+            },
+            dte="date",
+            time="timestamp",
+        )
+    elif isinstance(db, Lt):
+        db.create(
+            "test2",
+            dtypes={
+                "id": "integer primary key",
+                "score": "real",
+                "amt": "integer",
+                "cat": "text",
+            },
+            dte="text",
+            time="text",
+        )
+    elif isinstance(db, Oc):
+        db.create(
+            "test2",
+            dtypes={
+                "id": "number primary key",
+                "score": "float",
+                "amt": "number",
+                "cat": "varchar2(20)",
+            },
+            dte="date",
+            time="timestamp",
+        )
+    else:
+        raise ValueError
+
+    db.run("insert into test2 select * from test")
+    act = db.run("select * from test2 order by id")
+    exp = db.run("select * from test order by id")
+    assert_frame_equal_reset_index(act, exp)
+
+
+def test_db_opt_add_pkey(test_tbl, test_tbl2):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        db.run("create table test2 as select * from test")
+        db.add_pkey("test2", "id")
+    elif isinstance(db, Lt):
+        pass
+    elif isinstance(db, Oc):
+        pass
+    else:
+        raise ValueError
+
+
+def test_db_opt_create_schema(test_tbl, test_tbl2):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        try:
+            db.run("drop schema test cascade")
+        except Exception as ex:
+            if "does not exist" in str(ex):
+                pass
+            else:
+                raise (ex)
+        db.create_schema("test")
+        db.run("create table test.test (col int)")
+        db.run("drop schema test cascade")
+    elif isinstance(db, Lt):
+        pass
+    elif isinstance(db, Oc):
+        pass
+    else:
+        raise ValueError
+
+
+def test_db_opt_drop(test_tbl, test_tbl2):
+    db, df = test_tbl
+    db.run("create table test2 as select * from test")
+    db.drop("test2")
+    with pytest.raises(Exception) as e_info:
+        db.run("select count(1) from test2")
+
+
+def test_db_opt_write_nodup(test_tbl, test_tbl2):
+    db, df = test_tbl
+    db.run("create table test2 as select * from test where 1=2")
+    if isinstance(db, Pg):
+        db.write(df, "test2")
+        db.write_nodup(df, "test2", ["id"])
+        tbl = db.run("select * from test2 order by id")
+        assert_frame_equal_reset_index(tbl, df)
+    elif isinstance(db, Lt):
+        db.write(
+            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
+            "test2",
+        )
+        db.write_nodup(
+            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
+            "test2",
+            ["id"],
+        )
+        tbl = (
+            db.qry("test2")
+            .run()
+            .assign(
+                dte=lambda x: x["dte"].apply(
+                    lambda x: datetime.date.fromisoformat(x) if x else None
+                ),
+                time=lambda x: pd.to_datetime(x.time),
+            )
+        )
+        assert_frame_equal_reset_index(tbl, df)
+    elif isinstance(db, Oc):
+        db.write(
+            df,
+            "test2",
+        )
+        db.write_nodup(
+            df,
+            "test2",
+            ["id"],
+        )
+        tbl = db.run("select * from test2 order by id").assign(
+            dte=lambda x: x["dte"].apply(lambda x: x.date() if x else None)
+        )
+        df2 = df.assign(
+            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
+        )
+        assert_frame_equal_reset_index(tbl, df2)
+    else:
+        raise ValueError
+
+
+def test_db_opt_cwrite(test_tbl, test_tbl2):
+    db, df = test_tbl
+    if isinstance(db, Pg):
+        db.cwrite(df, "test2")
+        tbl = db.run("select * from test2 order by id").assign(
+            dte=lambda x: x["dte"].apply(
+                lambda x: datetime.date.fromisoformat(x) if x else None
+            )
+        )
+    elif isinstance(db, Lt):
+        db.cwrite(
+            df.assign(time=lambda x: x.time.astype(str).where(~x.time.isna(), None)),
+            "test2",
+        )
+        tbl = (
+            db.qry("test2")
+            .run()
+            .assign(
+                dte=lambda x: x["dte"].apply(
+                    lambda x: datetime.date.fromisoformat(x) if x else None
+                ),
+                time=lambda x: pd.to_datetime(x.time),
+            )
+        )
+    elif isinstance(db, Oc):
+        db.cwrite(
+            df,
+            "test2",
+        )
+        tbl = db.run("select * from test2 order by id").assign(
+            dte=lambda x: x["dte"].apply(
+                lambda x: datetime.datetime.strptime(x, "%d-%b-%y").date()
+                if x
+                else None
+            )
+        )
+        df = df.assign(
+            time=lambda x: x["time"].apply(lambda x: x.replace(microsecond=0))
+        )
+    else:
+        raise ValueError
+    assert_frame_equal_reset_index(tbl, df)
```

### Comparing `dwopt-0.0.7/tests/test_qry_cls.py` & `dwopt-0.0.8/tests/test_qry_cls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,157 @@
-from pandas.testing import assert_frame_equal
-from contextlib import redirect_stdout
-import io
-
-_SQL = "select count(1) from test"
-
-
-def test_qry_ops_run(test_tbl):
-    db, df = test_tbl
-    act = db.qry(sql=_SQL).run()
-    exp = db.run(_SQL)
-    assert_frame_equal(act, exp)
-
-
-def test_qry_ops_print(test_tbl):
-    db, df = test_tbl
-    with redirect_stdout(io.StringIO()) as f:
-        db.qry(sql=_SQL).print()
-    act = f.getvalue()
-    exp = _SQL
-    assert act.strip() == exp.strip()
-
-
-def test_qry_cls_select(test_tbl):
-    db, df = test_tbl
-
-    act = db.qry("test").select("id, score, amt").run()
-    exp = db.run(
-        """
-select id, score, amt
-from test
-    """
-    )
-    assert_frame_equal(act, exp)
-
-    act = db.qry("test").select("id", "score", "amt").run()
-    assert_frame_equal(act, exp)
-
-    act = db.qry("test").select(["id", "score", "amt"]).run()
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_case(test_tbl):
-    db, df = test_tbl
-    act = (
-        db.qry("test")
-        .select("test.*")
-        .case("col", "score >= 0.5 then 'A'", els="'B'")
-        .run()
-    )
-    exp = db.run(
-        """
-select test.*,
-    case when score >= 0.5 then 'A' else 'B' end as col
-from test
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_from_(test_tbl):
-    db, df = test_tbl
-    act = db.qry().from_("test").run()
-    exp = db.run("select * from test")
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_join(test_tbl):
-    db, df = test_tbl
-    act = (
-        db.qry("test x")
-        .select("x.id", "x.score", "y.score as scorey", "z.score as scorez")
-        .join("test y", "x.id = y.id+1")
-        .join("test z", "x.id = z.id+2")
-        .where("x.id <= 100")
-        .run()
-    )
-    exp = db.run(
-        """
-select 
-    x.id, x.score, y.score as scorey, z.score as scorez
-from test x
-left join test y on x.id = y.id+1
-left join test z on x.id = z.id+2
-where x.id <= 100
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_where(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").where("score > 0.5").run()
-    exp = db.run(
-        """
-select * from test where score > 0.5
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_group_by(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").select("cat, count(1) n").group_by("cat").run()
-    exp = db.run(
-        """
-select cat, count(1) as n
-from test
-group by cat
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_having(test_tbl):
-    db, df = test_tbl
-    act = (
-        db.qry("test")
-        .select("cat, count(1) n")
-        .group_by("cat")
-        .having("count(1) > 100")
-        .run()
-    )
-    exp = db.run(
-        """
-select cat, count(1) as n
-from test
-group by cat
-having count(1) > 100
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_order_by(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").order_by("id desc").run()
-    exp = db.run(
-        """
-select *
-from test
-order by id desc
-    """
-    )
-    assert_frame_equal(act, exp)
-
-
-def test_qry_cls_sql(test_tbl):
-    db, df = test_tbl
-    sql = """
-select * from test
-where score > 0.5
-    """
-    act = db.qry().sql(sql).run()
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
+import io
+from contextlib import redirect_stdout
+
+from pandas.testing import assert_frame_equal
+
+_SQL = "select count(1) from test"
+
+
+def test_qry_ops_run(test_tbl):
+    db, df = test_tbl
+    act = db.qry(sql=_SQL).run()
+    exp = db.run(_SQL)
+    assert_frame_equal(act, exp)
+
+
+def test_qry_ops_print(test_tbl):
+    db, df = test_tbl
+    with redirect_stdout(io.StringIO()) as f:
+        db.qry(sql=_SQL).print()
+    act = f.getvalue()
+    exp = _SQL
+    assert act.strip() == exp.strip()
+
+
+def test_qry_cls_select(test_tbl):
+    db, df = test_tbl
+
+    act = db.qry("test").select("id, score, amt").run()
+    exp = db.run(
+        """
+select id, score, amt
+from test
+    """
+    )
+    assert_frame_equal(act, exp)
+
+    act = db.qry("test").select("id", "score", "amt").run()
+    assert_frame_equal(act, exp)
+
+    act = db.qry("test").select(["id", "score", "amt"]).run()
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_case(test_tbl):
+    db, df = test_tbl
+    act = (
+        db.qry("test")
+        .select("test.*")
+        .case("col", "score >= 0.5 then 'A'", els="'B'")
+        .run()
+    )
+    exp = db.run(
+        """
+select test.*,
+    case when score >= 0.5 then 'A' else 'B' end as col
+from test
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_from_(test_tbl):
+    db, df = test_tbl
+    act = db.qry().from_("test").run()
+    exp = db.run("select * from test")
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_join(test_tbl):
+    db, df = test_tbl
+    act = (
+        db.qry("test x")
+        .select("x.id", "x.score", "y.score as scorey", "z.score as scorez")
+        .join("test y", "x.id = y.id+1")
+        .join("test z", "x.id = z.id+2")
+        .where("x.id <= 100")
+        .run()
+    )
+    exp = db.run(
+        """
+select 
+    x.id, x.score, y.score as scorey, z.score as scorez
+from test x
+left join test y on x.id = y.id+1
+left join test z on x.id = z.id+2
+where x.id <= 100
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_where(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").where("score > 0.5").run()
+    exp = db.run(
+        """
+select * from test where score > 0.5
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_group_by(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").select("cat, count(1) n").group_by("cat").run()
+    exp = db.run(
+        """
+select cat, count(1) as n
+from test
+group by cat
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_having(test_tbl):
+    db, df = test_tbl
+    act = (
+        db.qry("test")
+        .select("cat, count(1) n")
+        .group_by("cat")
+        .having("count(1) > 100")
+        .run()
+    )
+    exp = db.run(
+        """
+select cat, count(1) as n
+from test
+group by cat
+having count(1) > 100
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_order_by(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").order_by("id desc").run()
+    exp = db.run(
+        """
+select *
+from test
+order by id desc
+    """
+    )
+    assert_frame_equal(act, exp)
+
+
+def test_qry_cls_sql(test_tbl):
+    db, df = test_tbl
+    sql = """
+select * from test
+where score > 0.5
+    """
+    act = db.qry().sql(sql).run()
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
```

### Comparing `dwopt-0.0.7/tests/test_qry_sum.py` & `dwopt-0.0.8/tests/test_qry_sum.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from pandas.testing import assert_frame_equal, assert_series_equal
-
-from dwopt import Oc
-
-
-def test_qry_sum_top(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").order_by("id").top()
-    exp = db.run("select * from test where id = 0").iloc[0, :]
-    assert_series_equal(act, exp)
-
-
-def test_qry_sum_cols(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").cols()
-    exp = df.columns.tolist()
-    assert act == exp
-
-
-def test_qry_sum_head(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").order_by("id").head()
-    exp = db.run("select * from test where id < 5")
-    assert_frame_equal(act, exp)
-
-
-def test_qry_sum_len(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").len()
-    exp = df.shape[0]
-    assert act == exp
-
-
-def test_qry_sum_dist(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").dist("id")[0]
-    exp = df.loc[:, "id"].nunique()
-    assert act == exp
-
-
-def test_qry_sum_mimx(test_tbl):
-    db, df = test_tbl
-    act = db.qry("test").mimx("amt").tolist()
-    exp = [df.loc[:, "amt"].max(), df.loc[:, "amt"].min()]
-    assert act == exp
-
-
-def test_qry_sum_valc(test_tbl):
-    db, df = test_tbl
-    sql = """
-select cat,count(1) as n
-from test
-group by cat
-order by n desc
-    """
-    act = db.qry("test").valc("cat")
-    exp = db.run(sql)
-    assert_frame_equal(act, exp)
-
-
-def test_qry_sum_hash(test_tbl):
-    db, df = test_tbl
-    sql = """
-select
-    ora_hash(sum(ora_hash(
-        id || '_' || cat
-    ) - 4294967296/2)) hash
-from test
-    """
-    if isinstance(db, Oc):
-        act = db.qry("test").hash("id", "cat")
-        exp = db.run(sql).iloc[0, 0]
-        assert act == exp
-    else:
-        assert True
-        return
+from pandas.testing import assert_frame_equal, assert_series_equal
+
+from dwopt import Oc
+
+
+def test_qry_sum_top(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").order_by("id").top()
+    exp = db.run("select * from test where id = 0").iloc[0, :]
+    assert_series_equal(act, exp)
+
+
+def test_qry_sum_cols(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").cols()
+    exp = df.columns.tolist()
+    assert act == exp
+
+
+def test_qry_sum_head(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").order_by("id").head()
+    exp = db.run("select * from test where id < 5")
+    assert_frame_equal(act, exp)
+
+
+def test_qry_sum_len(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").len()
+    exp = df.shape[0]
+    assert act == exp
+
+
+def test_qry_sum_dist(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").dist("id")[0]
+    exp = df.loc[:, "id"].nunique()
+    assert act == exp
+
+
+def test_qry_sum_mimx(test_tbl):
+    db, df = test_tbl
+    act = db.qry("test").mimx("amt").tolist()
+    exp = [df.loc[:, "amt"].max(), df.loc[:, "amt"].min()]
+    assert act == exp
+
+
+def test_qry_sum_valc(test_tbl):
+    db, df = test_tbl
+    sql = """
+select cat,count(1) as n
+from test
+group by cat
+order by n desc
+    """
+    act = db.qry("test").valc("cat")
+    exp = db.run(sql)
+    assert_frame_equal(act, exp)
+
+
+def test_qry_sum_hash(test_tbl):
+    db, df = test_tbl
+    sql = """
+select
+    ora_hash(sum(ora_hash(
+        id || '_' || cat
+    ) - 4294967296/2)) hash
+from test
+    """
+    if isinstance(db, Oc):
+        act = db.qry("test").hash("id", "cat")
+        exp = db.run(sql).iloc[0, 0]
+        assert act == exp
+    else:
+        assert True
+        return
```

