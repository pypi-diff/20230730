# Comparing `tmp/changelog-generator-0.3.2.tar.gz` & `tmp/changelog_generator-0.7b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog-generator-0.3.2.tar", last modified: Sun Dec 18 21:57:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

