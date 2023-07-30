# Comparing `tmp/poetry_add_requirements_txt-1.1.2.tar.gz` & `tmp/poetry_add_requirements_txt-1.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_add_requirements_txt-1.1.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

