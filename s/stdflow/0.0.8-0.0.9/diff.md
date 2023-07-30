# Comparing `tmp/stdflow-0.0.8.tar.gz` & `tmp/stdflow-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cyprien/Documents/artefact/stdflow/dist/.tmp-jzu1q9wv/stdflow-0.0.8.tar", last modified: Thu Jul 27 08:59:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

