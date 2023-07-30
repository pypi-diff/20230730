# Comparing `tmp/prettier_prints-0.1.0.tar.gz` & `tmp/prettier_prints-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettier_prints-0.1.0.tar", last modified: Sun Jul 30 13:19:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

