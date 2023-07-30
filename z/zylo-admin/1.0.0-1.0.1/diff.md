# Comparing `tmp/zylo-admin-1.0.0.tar.gz` & `tmp/zylo_admin-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-admin-1.0.0.tar", last modified: Fri Jul 14 09:44:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

