# Comparing `tmp/ultibi-0.4.1.tar.gz` & `tmp/ultibi-0.4.2.tar.gz`

## Comparing `ultibi-0.4.1.tar` & `ultibi-0.4.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      754 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6456 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1243 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1418 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      358 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2292 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11847 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9484 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7614 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123    10170 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     4151 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123       40 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/mod.rs
--rw-r--r--   0     1001      123      349 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/sbm/equity.rs
--rw-r--r--   0     1001      123       12 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/sbm/mod.rs
--rw-r--r--   0     1001      123    26569 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5421 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14537 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13888 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3704 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7443 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    30238 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9869 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19328 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17723 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3846 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11817 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15622 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12479 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8796 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15266 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13490 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8074 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17062 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10966 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10440 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14299 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    12009 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10230 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14040 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21914 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15734 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5180 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1846 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1832 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1520 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4453 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18951 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      710 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4782 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     2903 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/datasource.rs
--rw-r--r--   0     1001      123    10820 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/mod.rs
--rw-r--r--   0     1001      123     2156 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/new.rs
--rw-r--r--   0     1001      123      700 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10937 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4628 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      478 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2663 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      588 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123     1413 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/awss3.rs
--rw-r--r--   0     1001      123     6085 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/helpers.rs
--rw-r--r--   0     1001      123     6863 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/mod.rs
--rw-r--r--   0     1001      123      371 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11951 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     3362 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      222 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/mod.rs
--rw-r--r--   0     1001      123     3332 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/report.rs
--rw-r--r--   0     1001      123     1870 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      734 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1441 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2210 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1269 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3094 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1417 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123     1056 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0     1001      123     1144 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/source.rs
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       98 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.4.1/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-07-24 19:30:20.000000 ultibi-0.4.1/.gitignore
--rw-r--r--   0     1001      123     5129 2023-07-24 19:30:20.000000 ultibi-0.4.1/LICENSE
--rw-r--r--   0     1001      123     2405 2023-07-24 19:30:20.000000 ultibi-0.4.1/Makefile
--rw-r--r--   0     1001      123     7071 2023-07-24 19:30:20.000000 ultibi-0.4.1/README.md
--rw-r--r--   0     1001      123     1559 2023-07-24 19:30:20.000000 ultibi-0.4.1/example.py
--rw-r--r--   0     1001      123     2098 2023-07-24 19:30:20.000000 ultibi-0.4.1/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-07-24 19:30:20.000000 ultibi-0.4.1/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-07-24 19:30:20.000000 ultibi-0.4.1/requirements.txt
--rw-r--r--   0     1001      123     3922 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3570 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     9008 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/dataset.rs
--rw-r--r--   0     1001      123     1786 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/datasource.rs
--rw-r--r--   0     1001      123     3833 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/filter.rs
--rw-r--r--   0     1001      123     2170 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123     1613 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1692 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_ds.py
--rw-r--r--   0     1001      123      826 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_filters.py
--rw-r--r--   0     1001      123     2658 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      878 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_source.py
--rw-r--r--   0     1001      123      918 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/__init__.py
--rw-r--r--   0     1001      123     1145 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     7999 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     2730 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/datasource.py
--rw-r--r--   0     1001      123     3257 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     8407 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2950 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   121869 2023-07-24 19:31:51.000000 ultibi-0.4.1/Cargo.lock
--rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 ultibi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 ultibi-0.4.2/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       98 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 ultibi-0.4.2/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4782 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     2903 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/datasource.rs
+-rw-r--r--   0     1001      123    10820 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/mod.rs
+-rw-r--r--   0     1001      123     2156 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/new.rs
+-rw-r--r--   0     1001      123      700 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10937 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4628 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      478 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2663 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      588 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123     1413 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/io/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/io/awss3.rs
+-rw-r--r--   0     1001      123     6085 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/io/helpers.rs
+-rw-r--r--   0     1001      123     6863 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/io/mod.rs
+-rw-r--r--   0     1001      123      371 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11951 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     3362 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      222 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123     3332 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1870 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      734 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1441 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2210 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1269 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3094 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1417 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123     1056 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0     1001      123     1144 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_core/tests/source.rs
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ultibi-0.4.2/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      754 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6456 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1243 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1418 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      358 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.4.2/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2292 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11847 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9484 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7614 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123    10170 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     4146 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123       40 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/reports/mod.rs
+-rw-r--r--   0     1001      123      349 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/reports/sbm/equity.rs
+-rw-r--r--   0     1001      123       12 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/reports/sbm/mod.rs
+-rw-r--r--   0     1001      123    26569 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5421 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14537 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13888 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3704 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7443 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    30251 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9869 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19328 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17723 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3846 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11817 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15622 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12479 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8796 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15266 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13490 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8074 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17062 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10966 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10440 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14299 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    12009 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10230 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14040 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21914 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15734 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5180 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1846 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1832 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1520 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4453 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18951 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      710 2023-07-30 14:38:12.000000 ultibi-0.4.2/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.4.2/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-07-30 14:38:12.000000 ultibi-0.4.2/.gitignore
+-rw-r--r--   0     1001      123     5129 2023-07-30 14:38:12.000000 ultibi-0.4.2/LICENSE
+-rw-r--r--   0     1001      123     2418 2023-07-30 14:38:12.000000 ultibi-0.4.2/Makefile
+-rw-r--r--   0     1001      123     7071 2023-07-30 14:38:12.000000 ultibi-0.4.2/README.md
+-rw-r--r--   0     1001      123     1559 2023-07-30 14:38:12.000000 ultibi-0.4.2/example.py
+-rw-r--r--   0     1001      123     2120 2023-07-30 14:38:12.000000 ultibi-0.4.2/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-07-30 14:38:12.000000 ultibi-0.4.2/requirements-lint.txt
+-rw-r--r--   0     1001      123      299 2023-07-30 14:38:12.000000 ultibi-0.4.2/requirements.txt
+-rw-r--r--   0     1001      123     3922 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3570 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     9008 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/dataset.rs
+-rw-r--r--   0     1001      123     1786 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/datasource.rs
+-rw-r--r--   0     1001      123     3833 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/filter.rs
+-rw-r--r--   0     1001      123     2170 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-07-30 14:38:12.000000 ultibi-0.4.2/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123     1613 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1692 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123      826 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/unit/test_filters.py
+-rw-r--r--   0     1001      123     2658 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      878 2023-07-30 14:38:12.000000 ultibi-0.4.2/tests/unit/test_source.py
+-rw-r--r--   0     1001      123      935 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1145 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     8000 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     2730 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/datasource.py
+-rw-r--r--   0     1001      123     3257 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     8407 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2950 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-07-30 14:38:12.000000 ultibi-0.4.2/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   121855 2023-07-30 14:39:54.000000 ultibi-0.4.2/Cargo.lock
+-rw-r--r--   0        0        0     8010 1970-01-01 00:00:00.000000 ultibi-0.4.2/PKG-INFO
```

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.4.2/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.4.1"
+version= "0.4.2"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.4.2/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.4.2/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.4.2/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.4.2/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.4.2/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.4.2/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "frtb_engine"
-version= "0.4.1"
+version= "0.4.2"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.4.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/measures.rs`

 * *Files 0% similar despite different names*

```diff
@@ -46,30 +46,30 @@
 
 use crate::drc::totals::drc_total_measures;
 
 use crate::rrao::rrao_measures;
 
 use crate::totals::sa_total_measures;
 
-use crate::prelude::total_delta_sens;
+use crate::prelude::total_sensis_sum;
 use ultibi::CPM;
 
 /// Exporting Measures
 pub(crate) fn frtb_measure_vec() -> Vec<Measure> {
     let non_rc_specific = vec![
         Measure::Base(BaseMeasure {
             name: "RiskWeights".to_string(),
             calculator: std::sync::Arc::new(sens_weights),
             aggregation: Some("first".into()),
             precomputefilter: None,
             calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "Total DeltaSens".to_string(),
-            calculator: std::sync::Arc::new(|_: &CPM| Ok(total_delta_sens())),
+            name: "Total Sens".to_string(),
+            calculator: std::sync::Arc::new(|_: &CPM| Ok(total_sensis_sum())),
             aggregation: None,
             precomputefilter: None,
             calc_params: vec![],
         }),
     ];
 
     let mut res = vec![];
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput, MeltArgs},
     BaseMeasure, DataFrame, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_commodity_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "Commodity", total_delta_sens()))
+    Ok(rc_rcat_sens("Delta", "Commodity", total_sensis_sum()))
 }
 
 /// Total Commodity Delta
 pub(crate) fn commodity_delta_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
     total_commodity_delta_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
 }
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     prelude::IntoParallelRefIterator,
 };
 use std::mem::MaybeUninit as MU;
 use std::sync::{Arc, Mutex};
 
 use crate::prelude::{RhoOverwrite, RhoType};
 
-/// Sum of all delta sensis, from spot to 30Y tenor
+/// Sum of all sensis, across all tenors, from spot to 30Y tenor
 /// In practice should be used only with filter on RiskClass
 /// as combining FX and IR sensis is meaningless
-pub fn total_delta_sens() -> Expr {
+pub fn total_sensis_sum() -> Expr {
     // When adding Exprs NULLs have to be filled Otherwise returns NULL
     col("SensitivitySpot").fill_null(0.)
         + col("Sensitivity_025Y").fill_null(0.)
         + col("Sensitivity_05Y").fill_null(0.)
         + col("Sensitivity_1Y").fill_null(0.)
         + col("Sensitivity_2Y").fill_null(0.)
         + col("Sensitivity_3Y").fill_null(0.)
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         &[col("RiskClass"), col("PnL_Up"), col("PnL_Down"), risk],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
 pub(crate) fn total_sens_curv_weighted() -> Expr {
-    total_delta_sens() * col("CurvatureRiskWeight")
+    total_sensis_sum() * col("CurvatureRiskWeight")
 }
 
 /// CSR
 pub(crate) fn cvr_up_5() -> Expr {
     lit::<f64>(0.) - (col("PnL_Up") - total_vega_curv_sens() * col("CurvatureRiskWeight"))
 }
 
@@ -98,15 +98,15 @@
         Cvr::Up => cvr_up_5(),
         Cvr::Down => cvr_down_5(),
     };
     rc_sens(rc, cvr)
 }
 
 pub(crate) fn curv_delta_total(rc: &'static str) -> Expr {
-    curv_delta(rc, total_delta_sens())
+    curv_delta(rc, total_sensis_sum())
 }
 
 pub(crate) fn curv_delta_spot(rc: &'static str) -> Expr {
     curv_delta(rc, col("SensitivitySpot"))
 }
 
 /// 5 tenors only
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use crate::helpers::*;
 use sbm::csr_nonsec::delta::csr_nonsec_delta_charge;
 use ultibi::{polars::prelude::max_horizontal, BaseMeasure, CPM};
 
 use crate::prelude::*;
 
 pub fn total_csr_sec_ctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "CSR_Sec_CTP", total_delta_sens()))
+    Ok(rc_rcat_sens("Delta", "CSR_Sec_CTP", total_sensis_sum()))
 }
 /// Helper functions
 
 fn csr_sec_ctp_delta_sens_weighted_05y_bcbs() -> Expr {
     rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_05Y", "SensWeights", 0)
 }
 fn csr_sec_ctp_delta_sens_weighted_1y_bcbs() -> Expr {
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput, MeltArgs},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_csr_sec_nonctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "CSR_Sec_nonCTP", total_delta_sens()))
+    Ok(rc_rcat_sens("Delta", "CSR_Sec_nonCTP", total_sensis_sum()))
 }
 /// Helper functions
 
 fn csr_sec_nonctp_delta_sens_weighted_05y_bcbs() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
         "CSR_Sec_nonCTP",
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //use polars::lazy::dsl::{apply_multiple, col, lit, when};
 use rayon::prelude::IntoParallelIterator;
 
 use crate::risk_weights::REDUCED_IR_WEIGHT;
 use ndarray::{parallel::prelude::ParallelIterator, Array1, Array2};
 
 pub fn total_ir_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "GIRR", total_delta_sens()))
+    Ok(rc_rcat_sens("Delta", "GIRR", total_sensis_sum()))
 }
 /// Helper functions
 fn girr_delta_sens_weighted_spot() -> Expr {
     rc_tenor_weighted_sens("Delta", "GIRR", "SensitivitySpot", "SensWeights", 0)
 }
 fn girr_delta_sens_weighted_025y() -> Expr {
     rc_tenor_weighted_sens("Delta", "GIRR", "Sensitivity_025Y", "SensWeights", 1)
```

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.4.2/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.4.2/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_core"
-version= "0.4.1"
+version= "0.4.2"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/datasource.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/mod.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/new.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/dataset/new.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/errors.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/acquire.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/io/acquire.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/awss3.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/io/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/helpers.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/io/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/mod.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/io/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/report.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/src/reports/report.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/overrides.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi_core/tests/source.rs` & `ultibi-0.4.2/local_dependencies/ultibi_core/tests/source.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/local_dependencies/ultibi/Cargo.toml` & `ultibi-0.4.2/local_dependencies/ultibi/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi"
-version= "0.4.1"
+version= "0.4.2"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.1/Cargo.toml` & `ultibi-0.4.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyultima"
-version= "0.4.1"
+version= "0.4.2"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
```

### Comparing `ultibi-0.4.1/.gitignore` & `ultibi-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/LICENSE` & `ultibi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/Makefile` & `ultibi-0.4.2/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 ifeq ($(OS),Windows_NT)
 	VENV_BIN=$(VENV)/Scripts
 else
 	VENV_BIN=$(VENV)/bin
 endif
 
-venv:  ## Set up virtual environment
-	python3 -m venv $(VENV)
+venv:  ## Set up virtual environment - local use
+	$(PY311) -m venv $(VENV)
 	$(VENV_BIN)/python -m pip install --upgrade pip
 	$(VENV_BIN)/pip install -r requirements.txt
 	$(VENV_BIN)/pip install -r requirements-lint.txt
 
 .PHONY: develop
 develop: venv  ## Compile and install Polars for development
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin develop
```

### Comparing `ultibi-0.4.1/README.md` & `ultibi-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/example.py` & `ultibi-0.4.2/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/pyproject.toml` & `ultibi-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 description = "Flexible DataFrame Operations via UI"
 readme = "README.md"
 authors = [
   { name = "Anatoly Bugakov", email = "anatoly@ultimabi.uk" },
 ]
 license = { file = "LICENSE" }
 dependencies = [
-  "polars >= 0.18.7",
+  "polars  >= 0.18.7",
+  "pyarrow >= 7.0.0"
 ]
 keywords = ["dataframe", "visualization", "aggregation", "calculation", 
   "chart", "data", "dataviz", "pivot-table", "frtb", "risk"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "License :: Free To Use But Restricted",
```

### Comparing `ultibi-0.4.1/src/calculator.rs` & `ultibi-0.4.2/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/conversions/series.rs` & `ultibi-0.4.2/src/conversions/series.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/conversions/wrappers.rs` & `ultibi-0.4.2/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/dataset.rs` & `ultibi-0.4.2/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/datasource.rs` & `ultibi-0.4.2/src/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/errors.rs` & `ultibi-0.4.2/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/filter.rs` & `ultibi-0.4.2/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/lib.rs` & `ultibi-0.4.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/measure.rs` & `ultibi-0.4.2/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/src/requests.rs` & `ultibi-0.4.2/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/data/datasource_config.toml` & `ultibi-0.4.2/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/docs/run_doc_examples.py` & `ultibi-0.4.2/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/unit/test_compute.py` & `ultibi-0.4.2/tests/unit/test_compute.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/unit/test_ds.py` & `ultibi-0.4.2/tests/unit/test_ds.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/unit/test_filters.py` & `ultibi-0.4.2/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/unit/test_measure.py` & `ultibi-0.4.2/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/tests/unit/test_source.py` & `ultibi-0.4.2/tests/unit/test_source.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/ultibi/__init__.py` & `ultibi-0.4.2/ultibi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 FRTB usecase specific library which levrages on ultima's base engine
 """
 
 import polars  # reexport
-import pyarrow
 
 from .internals import (
     AggRequest,
     BaseMeasure,
     CalcParam,
     ComputeRequest,
     CustomCalculator,
@@ -22,14 +21,17 @@
     NotInFilter,
     OtherError,
     StandardCalculator,
     UltimaError,
     aggregation_ops,
 )
 
+# import pyarrow - not needed
+
+
 __all__ = [
     "AggRequest",
     "ComputeRequest",
     "FRTBDataSet",
     "DataSet",
     "DataSource",
     "aggregation_ops",
```

### Comparing `ultibi-0.4.1/ultibi/internals/__init__.py` & `ultibi-0.4.2/ultibi/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/ultibi/internals/dataset.py` & `ultibi-0.4.2/ultibi/internals/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,37 +70,38 @@
     inner: DataSetWrapper
 
     def __init__(self, ds: DataSetWrapper) -> None:
         """
         Class constructor - not to br called directly.
         call .from_frame() or .from_config()
         """
+
         self.inner = ds
 
+        self.fields: list[str] = self.inner.fields()
         """All column which you can group by. Currently those are string 
             and bool columns
         """
-        self.fields: list[str] = self.inner.fields()
 
+        self.measures: "dict[str, str | None]" = self.inner.measures()
         """{measureName: "aggtype restriction(if any, otherwise
             None)"}. If none, then you can use any of the availiable agg operations.
             Check :func:`~ultima.internals.aggregation_ops` for supported aggregation
              operations
         """
-        self.measures: "dict[str, str | None]" = self.inner.measures()
 
+        self.calc_params: "list[tuple[str, str|None, str|None]]" = (
+            self.inner.calc_params()
+        )
         """parameters which you can pass to the Request for the given DataSet
 
         Returns:
             list[dict[str, str|None]]: List of {"name": parameter name to be
             passed to the request, "hint": type hint of the param}
         """
-        self.calc_params: "list[tuple[str, str|None, str|None]]" = (
-            self.inner.calc_params()
-        )
 
     @classmethod
     def from_config_path(cls: Type[DS], path: str) -> DS:
         """
         Reads path to <config>.toml
         Converts into DataSourceConfig
         Builds DataSet from DataSourceConfig
```

### Comparing `ultibi-0.4.1/ultibi/internals/datasource.py` & `ultibi-0.4.2/ultibi/internals/datasource.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/ultibi/internals/filters.py` & `ultibi-0.4.2/ultibi/internals/filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/ultibi/internals/measure.py` & `ultibi-0.4.2/ultibi/internals/measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/ultibi/internals/requests.py` & `ultibi-0.4.2/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.1/Cargo.lock` & `ultibi-0.4.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1427,17 +1427,17 @@
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_utils"
-version = "0.13.1"
+version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20ce151e1b790e3e36d767ae57691240feafe8b605e1c2fe081183d64ac1bff3"
+checksum = "9abcad25e9720609ccb3dcdb795d845e37d8ce34183330a9f48b03a1a71c8e21"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.27",
 ]
 
 [[package]]
@@ -1527,17 +1527,17 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+checksum = "6b30f669a7961ef1631673d2766cc92f52d64f7ef354d4fe0ddfd30ed52f0f4f"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
@@ -1648,15 +1648,15 @@
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -2166,27 +2166,27 @@
 name = "itoa"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jemalloc-sys"
-version = "0.5.3+5.3.0-patched"
+version = "0.5.4+5.3.0-patched"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9bd5d616ea7ed58b571b2e209a65759664d7fb021a0819d7a790afc67e47ca1"
+checksum = "ac6c1946e1cea1788cbfde01c993b52a10e2da07f4bac608228d1bed20bfebf2"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "jemallocator"
-version = "0.5.0"
+version = "0.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16c2514137880c52b0b4822b563fadd38257c1f380858addb74a400889696ea6"
+checksum = "a0de374a9f8e63150e6f5e8a60cc14c668226d7a347d8aee1a45766e3c4dd3bc"
 dependencies = [
  "jemalloc-sys",
  "libc",
 ]
 
 [[package]]
 name = "jobserver"
@@ -2327,17 +2327,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.10"
+version = "1.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24e6ab01971eb092ffe6a7d42f49f9ff42662f17604681e2843ad65077ba47dc"
+checksum = "d97137b25e321a73eef1418d1d5d2eda4d77e12813f8e6dead84bc52c5870a7b"
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
@@ -3366,15 +3366,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "ciborium",
  "frtb_engine",
  "once_cell",
  "polars",
  "pyo3",
  "serde_json",
@@ -3531,17 +3531,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax 0.7.4",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+checksum = "b7b6d6190b7594385f61bd3911cd1be99dfddcfc365a4160cc2ab5bff4aed294"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax 0.7.4",
 ]
 
 [[package]]
@@ -3678,21 +3678,20 @@
 dependencies = [
  "sha2",
  "walkdir",
 ]
 
 [[package]]
 name = "rust_decimal"
-version = "1.30.0"
+version = "1.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0446843641c69436765a35a5a77088e28c2e6a12da93e84aa3ab1cd4aa5a042"
+checksum = "4a2ab0025103a60ecaaf3abf24db1db240a4e1c15837090d2c32f625ac98abea"
 dependencies = [
  "arrayvec",
  "borsh",
- "bytecheck",
  "byteorder",
  "bytes",
  "num-traits",
  "postgres",
  "rand",
  "rkyv",
  "serde",
@@ -3852,37 +3851,37 @@
 name = "semver"
 version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.175"
+version = "1.0.178"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d25439cd7397d044e2748a6fe2432b5e85db703d6d097bd014b3c0ad1ebff0b"
+checksum = "60363bdd39a7be0266a520dab25fdc9241d2f987b08a01e01f0ec6d06a981348"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.175"
+version = "1.0.178"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b23f7ade6f110613c0d63858ddb8b94c1041f550eab58a16b371bdf2c9c80ab4"
+checksum = "f28482318d6641454cb273da158647922d1be6b5a2fcc6165cd89ebdd7ed576b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.103"
+version = "1.0.104"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
+checksum = "076066c5f1078eac5b722a31827a8832fe108bed65dfa75e233c89f8206e976c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -4172,17 +4171,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.29.6"
+version = "0.29.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7cb97a5a85a136d84e75d5c3cf89655090602efb1be0d8d5337b7e386af2908"
+checksum = "165d6d8539689e3d3bc8b98ac59541e1f21c7de7c85d60dc80e43ae0ed2113db"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "winapi",
@@ -4217,15 +4216,15 @@
  "redox_syscall 0.3.5",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -4564,23 +4563,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "connectorx",
  "dashmap",
  "derivative",
  "futures",
@@ -4593,15 +4592,15 @@
  "tokio",
  "toml 0.7.6",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -4985,17 +4984,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.5.0"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
+checksum = "8bd122eb777186e60c3fdf765a58ac76e41c582f1f535fbf3314434c6b58f3f7"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
```

### Comparing `ultibi-0.4.1/PKG-INFO` & `ultibi-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.4.1
+Version: 0.4.2
 Classifier: Programming Language :: Rust
 Classifier: License :: Free To Use But Restricted
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: polars >=0.18.7
+Requires-Dist: pyarrow >=7.0.0
 License-File: LICENSE
 Summary: Flexible DataFrame Operations via UI
 Keywords: dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-table,frtb,risk
 Author-email: Anatoly Bugakov <anatoly@ultimabi.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://ultimabi.uk/
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.4.1 Classifier: Programming
+Metadata-Version: 2.1 Name: ultibi Version: 0.4.2 Classifier: Programming
 Language :: Rust Classifier: License :: Free To Use But Restricted Classifier:
 Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polars >=0.18.7 License-File: LICENSE Summary: Flexible
-DataFrame Operations via UI Keywords:
+Requires-Dist: polars >=0.18.7 Requires-Dist: pyarrow >=7.0.0 License-File:
+LICENSE Summary: Flexible DataFrame Operations via UI Keywords:
 dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
 table,frtb,risk Author-email: Anatoly Bugakov
 ultimabi.uk> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: Homepage, https://ultimabi.uk/ Project-
 URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/ Project-URL:
 Repository, https://github.com/ultima-ib/ultibi-frtb-book
                                  [Ultima_Logo]
```

