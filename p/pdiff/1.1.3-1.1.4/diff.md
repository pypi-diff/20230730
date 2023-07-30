# Comparing `tmp/pdiff-1.1.3.tar.gz` & `tmp/pdiff-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdiff-1.1.3.tar", last modified: Sun Mar 26 23:46:31 2023, max compression
+gzip compressed data, was "pdiff-1.1.4.tar", last modified: Sun Jul 30 05:09:36 2023, max compression
```

## Comparing `pdiff-1.1.3.tar` & `pdiff-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2023-03-26 23:46:31.608529 pdiff-1.1.3/
--rw-r--r--   0 nkouevda   (501) staff       (20)     1058 2017-08-25 06:30:05.000000 pdiff-1.1.3/LICENSE.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)     1673 2023-03-26 23:46:31.608226 pdiff-1.1.3/PKG-INFO
--rw-r--r--   0 nkouevda   (501) staff       (20)     1409 2021-11-14 02:19:02.000000 pdiff-1.1.3/README.md
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2023-03-26 23:46:31.606186 pdiff-1.1.3/pdiff/
--rw-r--r--   0 nkouevda   (501) staff       (20)       37 2017-08-25 06:00:42.000000 pdiff-1.1.3/pdiff/__init__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      809 2023-03-26 23:46:24.000000 pdiff-1.1.3/pdiff/__main__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)       22 2023-03-26 23:45:17.000000 pdiff-1.1.3/pdiff/__version__.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     1753 2023-03-26 23:46:24.000000 pdiff-1.1.3/pdiff/argument_parser.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      639 2020-12-30 09:40:19.000000 pdiff-1.1.3/pdiff/colors.py
--rw-r--r--   0 nkouevda   (501) staff       (20)     6524 2023-03-26 23:46:24.000000 pdiff-1.1.3/pdiff/diff_formatter.py
--rw-r--r--   0 nkouevda   (501) staff       (20)      814 2020-03-09 02:13:29.000000 pdiff-1.1.3/pdiff/terminal_util.py
-drwxr-xr-x   0 nkouevda   (501) staff       (20)        0 2023-03-26 23:46:31.607907 pdiff-1.1.3/pdiff.egg-info/
--rw-r--r--   0 nkouevda   (501) staff       (20)     1673 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/PKG-INFO
--rw-r--r--   0 nkouevda   (501) staff       (20)      351 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/SOURCES.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)        1 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/dependency_links.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)       46 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/entry_points.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)        9 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/requires.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)        6 2023-03-26 23:46:31.000000 pdiff-1.1.3/pdiff.egg-info/top_level.txt
--rw-r--r--   0 nkouevda   (501) staff       (20)       38 2023-03-26 23:46:31.608604 pdiff-1.1.3/setup.cfg
--rw-r--r--   0 nkouevda   (501) staff       (20)      671 2021-01-02 00:51:21.000000 pdiff-1.1.3/setup.py
+drwxr-xr-x   0 nkouevda   (502) staff       (20)        0 2023-07-30 05:09:36.847580 pdiff-1.1.4/
+-rw-r--r--   0 nkouevda   (502) staff       (20)     1058 2017-08-25 06:30:05.000000 pdiff-1.1.4/LICENSE.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)     1674 2023-07-30 05:09:36.847481 pdiff-1.1.4/PKG-INFO
+-rw-r--r--   0 nkouevda   (502) staff       (20)     1410 2023-07-30 05:00:46.000000 pdiff-1.1.4/README.md
+drwxr-xr-x   0 nkouevda   (502) staff       (20)        0 2023-07-30 05:09:36.846741 pdiff-1.1.4/pdiff/
+-rw-r--r--   0 nkouevda   (502) staff       (20)       37 2017-08-25 06:00:42.000000 pdiff-1.1.4/pdiff/__init__.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)      815 2023-07-30 05:00:21.000000 pdiff-1.1.4/pdiff/__main__.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)       22 2023-07-30 05:07:03.000000 pdiff-1.1.4/pdiff/__version__.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)     1762 2023-07-30 05:00:35.000000 pdiff-1.1.4/pdiff/argument_parser.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)      639 2020-12-30 09:40:19.000000 pdiff-1.1.4/pdiff/colors.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)     6689 2023-07-30 05:00:07.000000 pdiff-1.1.4/pdiff/diff_formatter.py
+-rw-r--r--   0 nkouevda   (502) staff       (20)      814 2020-03-09 02:13:29.000000 pdiff-1.1.4/pdiff/terminal_util.py
+drwxr-xr-x   0 nkouevda   (502) staff       (20)        0 2023-07-30 05:09:36.847334 pdiff-1.1.4/pdiff.egg-info/
+-rw-r--r--   0 nkouevda   (502) staff       (20)     1674 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/PKG-INFO
+-rw-r--r--   0 nkouevda   (502) staff       (20)      351 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)        1 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)       46 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/entry_points.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)        9 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/requires.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)        6 2023-07-30 05:09:36.000000 pdiff-1.1.4/pdiff.egg-info/top_level.txt
+-rw-r--r--   0 nkouevda   (502) staff       (20)       38 2023-07-30 05:09:36.847607 pdiff-1.1.4/setup.cfg
+-rw-r--r--   0 nkouevda   (502) staff       (20)      671 2021-01-02 00:51:21.000000 pdiff-1.1.4/setup.py
```

### Comparing `pdiff-1.1.3/LICENSE.txt` & `pdiff-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdiff-1.1.3/PKG-INFO` & `pdiff-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdiff
-Version: 1.1.3
+Version: 1.1.4
 Summary: Pretty side-by-side diff
 Home-page: https://github.com/nkouevda/pdiff
 Author: Nikita Kouevda
 Author-email: nkouevda@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,28 +14,28 @@
 Pretty side-by-side diff.
 
 Inspired by [`ydiff`](https://github.com/ymattw/ydiff) and
 [`icdiff`](https://github.com/jeffkaufman/icdiff).
 
 ## Example
 
-![pdiff.png](https://github.com/nkouevda/images/raw/master/pdiff.png)
+![pdiff.png](https://github.com/nkouevda/images/raw/main/pdiff.png)
 
 ## Installation
 
     pip install pdiff
 
 Or:
 
     brew install nkouevda/nkouevda/pdiff
 
 ## Usage
 
 ```
-usage: pdiff [<options>] [--] <old file> <new file>
+usage: pdiff [<options>] [--] <left file> <right file>
 
 Pretty side-by-side diff
 
 optional arguments:
   -h, --help            show this help message and exit
   -b, --background, --no-background
                         highlight background instead of foreground (default: True)
```

### Comparing `pdiff-1.1.3/README.md` & `pdiff-1.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 Pretty side-by-side diff.
 
 Inspired by [`ydiff`](https://github.com/ymattw/ydiff) and
 [`icdiff`](https://github.com/jeffkaufman/icdiff).
 
 ## Example
 
-![pdiff.png](https://github.com/nkouevda/images/raw/master/pdiff.png)
+![pdiff.png](https://github.com/nkouevda/images/raw/main/pdiff.png)
 
 ## Installation
 
     pip install pdiff
 
 Or:
 
     brew install nkouevda/nkouevda/pdiff
 
 ## Usage
 
 ```
-usage: pdiff [<options>] [--] <old file> <new file>
+usage: pdiff [<options>] [--] <left file> <right file>
 
 Pretty side-by-side diff
 
 optional arguments:
   -h, --help            show this help message and exit
   -b, --background, --no-background
                         highlight background instead of foreground (default: True)
```

### Comparing `pdiff-1.1.3/pdiff/__main__.py` & `pdiff-1.1.4/pdiff/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from . import diff_formatter
 
 
 def main():
   parser = argument_parser.get_parser()
   args = parser.parse_args()
 
-  for filename in (args.old_filename, args.new_filename):
+  for filename in (args.left_filename, args.right_filename):
     if not os.path.exists(filename):
       sys.stderr.write('error: file does not exist: %s\n' % filename)
       return 1
     elif os.path.isdir(filename):
       sys.stderr.write('error: path is a directory: %s\n' % filename)
       return 1
 
   formatter = diff_formatter.DiffFormatter(
-      args.old_filename,
-      args.new_filename,
+      args.left_filename,
+      args.right_filename,
       args.context,
       args.width,
       args.tab_size,
       args.signs,
       args.line_numbers,
       args.background)
```

### Comparing `pdiff-1.1.3/pdiff/argument_parser.py` & `pdiff-1.1.4/pdiff/argument_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from . import __version__
 from . import terminal_util
 
 
 def get_parser():
   parser = argparse.ArgumentParser(
-      usage='%(prog)s [<options>] [--] <old file> <new file>',
+      usage='%(prog)s [<options>] [--] <left file> <right file>',
       description='Pretty side-by-side diff')
 
   parser.add_argument(
-      'old_filename',
+      'left_filename',
       type=str,
       help=argparse.SUPPRESS,
-      metavar='<old file>')
+      metavar='<left file>')
   parser.add_argument(
-      'new_filename',
+      'right_filename',
       type=str,
       help=argparse.SUPPRESS,
-      metavar='<new file>')
+      metavar='<right file>')
 
   parser.add_argument(
       '-b',
       '--background',
       action=argparse.BooleanOptionalAction,
       default=True,
       help='highlight background instead of foreground')
```

### Comparing `pdiff-1.1.3/pdiff/colors.py` & `pdiff-1.1.4/pdiff/colors.py`

 * *Files identical despite different names*

### Comparing `pdiff-1.1.3/pdiff/diff_formatter.py` & `pdiff-1.1.4/pdiff/diff_formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,72 +3,72 @@
 import re
 
 from . import colors
 
 
 class DiffFormatter(object):
 
-  OLD_HEADER_PREFIX = '--- '
-  NEW_HEADER_PREFIX = '+++ '
-  OLD_HUNK_HEADER_TEMPLATE = '@@ -%d,%d @@'
-  NEW_HUNK_HEADER_TEMPLATE = '@@ +%d,%d @@'
+  LEFT_HEADER_PREFIX = '--- '
+  RIGHT_HEADER_PREFIX = '+++ '
+  LEFT_HUNK_HEADER_TEMPLATE = '@@ -%d,%d @@'
+  RIGHT_HUNK_HEADER_TEMPLATE = '@@ +%d,%d @@'
 
   def __init__(
       self,
-      old_filename,
-      new_filename,
+      left_filename,
+      right_filename,
       context,
       width,
       tab_size,
       signs,
       line_numbers,
       background):
-    self.old_filename = old_filename
-    self.new_filename = new_filename
+    self.left_filename = left_filename
+    self.right_filename = right_filename
     self.context = context
     self.width = width
     self.tab_size = tab_size
     self.signs = signs
     self.line_numbers = line_numbers
     self.background = background
 
     self.half_width = self.width // 2 - 1
     self.empty_half = ' ' * self.half_width
     self.tab_spaces = ' ' * self.tab_size
     self.marker_to_colors = colors.MARKERS_BG if self.background else colors.MARKERS_FG
 
   def get_lines(self):
     # `readlines` because `difflib._mdiff` can't operate on a generator
-    with open(self.old_filename, 'r') as old_file:
-      old_lines = old_file.readlines()
-    with open(self.new_filename, 'r') as new_file:
-      new_lines = new_file.readlines()
+    with open(self.left_filename, 'r') as left_file:
+      left_lines = left_file.readlines()
+    with open(self.right_filename, 'r') as right_file:
+      right_lines = right_file.readlines()
 
     yield self._format_file_header()
 
     # Determine line number column widths; note: in some cases this is
     # unnecessarily wide (e.g. if changes only in beginning of a long file)
-    old_ln_width = len(str(len(old_lines)))
-    new_ln_width = len(str(len(new_lines)))
+    left_ln_width = len(str(len(left_lines)))
+    right_ln_width = len(str(len(right_lines)))
 
-    mdiff = difflib._mdiff(old_lines, new_lines, context=self.context)
+    mdiff = difflib._mdiff(left_lines, right_lines, context=self.context)
 
     # `mdiff` context separators don't have the metadata necessary to generate
     # git-diff-like hunk headers (`@@ -%d,%d @@` and `@@ +%d,%d @@`), so we
     # partition `mdiff` into hunks and process each one separately
     for hunk in self._get_hunks(mdiff):
-      for line in self._format_hunk(hunk, old_ln_width, new_ln_width):
+      for line in self._format_hunk(hunk, left_ln_width, right_ln_width):
         yield line
 
   def _format_file_header(self):
-    old_header = colors.colorize(
-        DiffFormatter.OLD_HEADER_PREFIX + self.old_filename, colors.FILE_HEADER)
-    new_header = colors.colorize(
-        DiffFormatter.NEW_HEADER_PREFIX + self.new_filename, colors.FILE_HEADER)
-    return self._format_line(old_header, new_header)
+    left_header = colors.colorize(
+        DiffFormatter.LEFT_HEADER_PREFIX + self.left_filename, colors.FILE_HEADER)
+    right_header = colors.colorize(
+        DiffFormatter.RIGHT_HEADER_PREFIX + self.right_filename, colors.FILE_HEADER)
+    return self._format_line(left_header, right_header)
 
   def _get_hunks(self, mdiff):
     hunk = []
 
     for mdiff_tuple in mdiff:
       if mdiff_tuple[2] is None:
         if hunk:
@@ -77,76 +77,76 @@
       else:
         hunk.append(mdiff_tuple)
 
     # Don't forget the last hunk, which isn't followed by a context separator
     if hunk:
       yield hunk
 
-  def _format_hunk(self, hunk, old_ln_width, new_ln_width):
+  def _format_hunk(self, hunk, left_ln_width, right_ln_width):
     yield self._format_hunk_header(hunk)
 
-    for (old_num, old_half), (new_num, new_half), has_changes in hunk:
-      old_half = old_half.replace('\n', '').replace('\t', self.tab_spaces)
-      new_half = new_half.replace('\n', '').replace('\t', self.tab_spaces)
+    for (left_num, left_half), (right_num, right_half), has_changes in hunk:
+      left_half = left_half.replace('\n', '').replace('\t', self.tab_spaces)
+      right_half = right_half.replace('\n', '').replace('\t', self.tab_spaces)
 
       if has_changes:
         for marker, color in self.marker_to_colors.items():
-          old_half = old_half.replace(marker, color)
-          new_half = new_half.replace(marker, color)
+          left_half = left_half.replace(marker, color)
+          right_half = right_half.replace(marker, color)
 
         # Use background color for whitespace-only diffs even if no --background
-        if old_half and new_half and not self.background:
-          old_half = self._highlight_whitespace_background(old_half)
-          new_half = self._highlight_whitespace_background(new_half)
+        if left_half and right_half and not self.background:
+          left_half = self._highlight_whitespace_background(left_half)
+          right_half = self._highlight_whitespace_background(right_half)
 
-      old_sign, new_sign = self._format_signs(old_half, new_half, has_changes)
+      left_sign, right_sign = self._format_signs(left_half, right_half, has_changes)
 
       if self.line_numbers:
-        old_half = str(old_num).rjust(old_ln_width) + ' ' + old_half
-        new_half = str(new_num).rjust(new_ln_width) + ' ' + new_half
+        left_half = str(left_num).rjust(left_ln_width) + ' ' + left_half
+        right_half = str(right_num).rjust(right_ln_width) + ' ' + right_half
 
-      yield self._format_line(old_sign + old_half, new_sign + new_half)
+      yield self._format_line(left_sign + left_half, right_sign + right_half)
 
   def _format_hunk_header(self, hunk):
-    old_nums = [old_num for (old_num, _), _, _ in hunk if old_num != '']
-    new_nums = [new_num for _, (new_num, _), _ in hunk if new_num != '']
-    old_start = old_nums[0] if old_nums else 0
-    new_start = new_nums[0] if new_nums else 0
-    old_header = colors.colorize(
-        DiffFormatter.OLD_HUNK_HEADER_TEMPLATE % (old_start, len(old_nums)),
+    left_nums = [left_num for (left_num, _), _, _ in hunk if left_num != '']
+    right_nums = [right_num for _, (right_num, _), _ in hunk if right_num != '']
+    left_start = left_nums[0] if left_nums else 0
+    right_start = right_nums[0] if right_nums else 0
+    left_header = colors.colorize(
+        DiffFormatter.LEFT_HUNK_HEADER_TEMPLATE % (left_start, len(left_nums)),
         colors.HUNK_HEADER)
-    new_header = colors.colorize(
-        DiffFormatter.NEW_HUNK_HEADER_TEMPLATE % (new_start, len(new_nums)),
+    right_header = colors.colorize(
+        DiffFormatter.RIGHT_HUNK_HEADER_TEMPLATE % (right_start, len(right_nums)),
         colors.HUNK_HEADER)
-    return self._format_line(old_header, new_header)
+    return self._format_line(left_header, right_header)
 
   def _highlight_whitespace_background(self, line):
     # For whitespace-only diffs, change `\x1b[30m` to `\x1b[40m` (background)
     return re.sub('(?<=\x1b\\[)3(?=[0-7]m\\s+\x1b\\[0m)', '4', line)
 
-  def _format_signs(self, old_half, new_half, has_changes):
+  def _format_signs(self, left_half, right_half, has_changes):
     if not self.signs:
       return '', ''
     if not has_changes:
       return '  ', '  '
-    elif not old_half:
+    elif not left_half:
       return '  ', colors.colorize('+ ', colors.ADD_FG)
-    elif not new_half:
+    elif not right_half:
       return colors.colorize('- ', colors.DELETE_FG), '  '
     else:
       return (colors.colorize('! ', colors.CHANGE_FG),) * 2
 
-  def _format_line(self, old_half, new_half):
-    old_half_lines = self._format_half_lines(old_half)
-    new_half_lines = self._format_half_lines(new_half)
+  def _format_line(self, left_half, right_half):
+    left_half_lines = self._format_half_lines(left_half)
+    right_half_lines = self._format_half_lines(right_half)
 
     return '\n'.join(
-        old_half + ' ' + new_half
-        for old_half, new_half in itertools.zip_longest(
-            old_half_lines, new_half_lines, fillvalue=self.empty_half)) + '\n'
+        left_half + ' ' + right_half
+        for left_half, right_half in itertools.zip_longest(
+            left_half_lines, right_half_lines, fillvalue=self.empty_half)) + '\n'
 
   def _format_half_lines(self, half_line):
     # Split `'ab\x1b[31mcd\x1b[0m'` into `['ab', '\x1b[31m', 'cd', '\x1b[0m']`
     parts = re.split('(\x1b\\[(?:0|[34][0-7])m)', half_line)
     visible_len = sum(len(part) for part in parts if not part.startswith('\x1b'))
 
     if visible_len <= self.half_width:
```

### Comparing `pdiff-1.1.3/pdiff/terminal_util.py` & `pdiff-1.1.4/pdiff/terminal_util.py`

 * *Files identical despite different names*

### Comparing `pdiff-1.1.3/pdiff.egg-info/PKG-INFO` & `pdiff-1.1.4/pdiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdiff
-Version: 1.1.3
+Version: 1.1.4
 Summary: Pretty side-by-side diff
 Home-page: https://github.com/nkouevda/pdiff
 Author: Nikita Kouevda
 Author-email: nkouevda@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,28 +14,28 @@
 Pretty side-by-side diff.
 
 Inspired by [`ydiff`](https://github.com/ymattw/ydiff) and
 [`icdiff`](https://github.com/jeffkaufman/icdiff).
 
 ## Example
 
-![pdiff.png](https://github.com/nkouevda/images/raw/master/pdiff.png)
+![pdiff.png](https://github.com/nkouevda/images/raw/main/pdiff.png)
 
 ## Installation
 
     pip install pdiff
 
 Or:
 
     brew install nkouevda/nkouevda/pdiff
 
 ## Usage
 
 ```
-usage: pdiff [<options>] [--] <old file> <new file>
+usage: pdiff [<options>] [--] <left file> <right file>
 
 Pretty side-by-side diff
 
 optional arguments:
   -h, --help            show this help message and exit
   -b, --background, --no-background
                         highlight background instead of foreground (default: True)
```

### Comparing `pdiff-1.1.3/setup.py` & `pdiff-1.1.4/setup.py`

 * *Files identical despite different names*

