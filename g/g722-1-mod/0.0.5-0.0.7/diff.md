# Comparing `tmp/g722_1_mod-0.0.5.tar.gz` & `tmp/g722_1_mod-0.0.7-pp37-pypy37_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g722_1_mod-0.0.5.tar", last modified: Wed Jul  5 20:12:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

