# Comparing `tmp/toui-3.0.3.tar.gz` & `tmp/toui-3.0.3b0-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.0.3.tar", last modified: Sat Jul 29 20:20:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

