# Comparing `tmp/HTML_String_Tools-0.1.0-py3-none-any.whl.zip` & `tmp/HTML_String_Tools-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 17804 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       23 b- defN 22-May-04 21:31 html_string_tools/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 22-May-04 21:31 html_string_tools/main/__init__.py
--rw-rw-r--  2.0 unx     5875 b- defN 22-May-06 21:01 html_string_tools/main/html_string_tools.py
--rw-rw-r--  2.0 unx       23 b- defN 22-May-04 21:31 html_string_tools/test/__init__.py
--rw-rw-r--  2.0 unx     7150 b- defN 22-May-06 21:01 html_string_tools/test/test_html_string_tools.py
--rw-rw-r--  2.0 unx    35149 b- defN 22-May-09 18:08 HTML_String_Tools-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 22-May-09 18:08 HTML_String_Tools-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-09 18:08 HTML_String_Tools-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 22-May-09 18:08 HTML_String_Tools-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      903 b- defN 22-May-09 18:08 HTML_String_Tools-0.1.0.dist-info/RECORD
-10 files, 49899 bytes uncompressed, 16228 bytes compressed:  67.5%
+Zip file size: 18285 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-30 20:15 html_string_tools/__init__.py
+-rw-r--r--  2.0 unx     4116 b- defN 23-Jul-30 20:39 html_string_tools/html.py
+-rw-r--r--  2.0 unx     1806 b- defN 23-Jul-30 20:26 html_string_tools/regex.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-30 19:29 html_string_tools/tests/__init__.py
+-rw-r--r--  2.0 unx     5761 b- defN 23-Jul-30 20:43 html_string_tools/tests/test_html.py
+-rw-r--r--  2.0 unx     1749 b- defN 23-Jul-30 20:29 html_string_tools/tests/test_regex.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-30 20:47 HTML_String_Tools-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      606 b- defN 23-Jul-30 20:47 HTML_String_Tools-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 20:47 HTML_String_Tools-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-30 20:47 HTML_String_Tools-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jul-30 20:47 HTML_String_Tools-0.2.0.dist-info/RECORD
+11 files, 50304 bytes uncompressed, 16633 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: html_string_tools/__init__.py
 Comment: 
 
-Filename: html_string_tools/main/__init__.py
+Filename: html_string_tools/html.py
 Comment: 
 
-Filename: html_string_tools/main/html_string_tools.py
+Filename: html_string_tools/regex.py
 Comment: 
 
-Filename: html_string_tools/test/__init__.py
+Filename: html_string_tools/tests/__init__.py
 Comment: 
 
-Filename: html_string_tools/test/test_html_string_tools.py
+Filename: html_string_tools/tests/test_html.py
 Comment: 
 
-Filename: HTML_String_Tools-0.1.0.dist-info/LICENSE
+Filename: html_string_tools/tests/test_regex.py
 Comment: 
 
-Filename: HTML_String_Tools-0.1.0.dist-info/METADATA
+Filename: HTML_String_Tools-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: HTML_String_Tools-0.1.0.dist-info/WHEEL
+Filename: HTML_String_Tools-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: HTML_String_Tools-0.1.0.dist-info/top_level.txt
+Filename: HTML_String_Tools-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: HTML_String_Tools-0.1.0.dist-info/RECORD
+Filename: HTML_String_Tools-0.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: HTML_String_Tools-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## html_string_tools/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3
```

## Comparing `html_string_tools/main/html_string_tools.py` & `html_string_tools/html.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,26 @@
-#!/usr/bin/env
+#!/usr/bin/env python3
 
-from html import unescape
-from re import findall as re_find
-from re import sub as re_sub
-
-def regex_replace(funct, pattern:str, string:str) -> str:
-    """
-    Replaces text matching regex pattern with said matching text run though a given function.
-
-    :param funct: Function to run matching text through, required
-    :type funct: function, required
-    :param pattern: Regex pattern to search for in string
-    :type pattern: str, required
-    :param string: String to search for pattern within
-    :type string: str, required
-    :return: Given string with pattern matched text replaced
-    :rtype: str
-    """
-    try:
-        # Get all strings that match the regex pattern
-        matches = re_find(pattern, string)
-        # Run through all matches to replace text
-        new_text = ""
-        left_text = string
-        for match in matches:
-            # Keep all of the text begore the match
-            index = left_text.find(match)
-            new_text = new_text + left_text[:index]
-            # Add replacement for the match
-            new_text = new_text + funct(match)
-            # Set the remaining text for after the match
-            index += len(match)
-            left_text = left_text[index:]
-        # Keep all the text left in the initial string
-        new_text = new_text + left_text
-        # Return the string with matching patterns replaced
-        return new_text
-    except TypeError: return string
-
-def remove_whitespace(string:str) -> str:
-    """
-    Removes whitespace from the beggining and end of a given string.
-
-    :param string: Given string to remove whitespace from
-    :type string: str, required
-    :return: String with the whitespace removed
-    :rtype: str
-    """
-    try:
-        # Remove leading and ending whitespace
-        return re_sub("^\\s+|\\s+$", "", string)
-    except TypeError: return string
+import re
+import html
+from . import regex
 
 def get_extension(path:str) -> str:
     """
     Returns the extension for a given filename or direct file URL.
     If extension does not exist, returns empty.
 
     :param path: Given path with extension
     :type path: str, required
     :return: Extension for the path
     :rtype: str
     """
     try:
         # Find potential extensions
-        match = re_find("\\.[a-zA-Z0-9]{1,5}\\?|\\.[a-zA-Z0-9]{1,5}$", path)
+        match = re.findall("\\.[a-zA-Z0-9]{1,5}\\?|\\.[a-zA-Z0-9]{1,5}$", path)
         # Remove "?" from end of extension, if necessary
         extension = match[0]
         for item in match:
             if item.endswith("?"):
                 extension = item[:len(item)-1]
         # Return the extension
         return extension
@@ -82,81 +34,81 @@
     :param escape: HTML escape character
     :type escape: str, required
     :return: Unicode character
     :rtype: str
     """
     try:
         # Check that the given string is an HTML entity
-        return unescape(re_find("^&[^&;]+;$", entity)[0])
+        return html.unescape(re.findall("^&[^&;]+;$", entity)[0])
     except (IndexError, TypeError): return entity
 
-def replace_entities(string:str=None) -> str:
-    """
-    Replaces all HTML entities in a string with Unicode characters.
-
-    :param string: Given string
-    :type string: str, required
-    :return: String with HTML escape characters replaced
-    :rtype: str
-    """
-    return regex_replace(entity_to_character, "&[^&;]+;", string)
-
 def character_to_entity(character:str) -> str:
     """
     Converts a single character into an HTML entity.
 
     :param character: Single character to convert into an HTML escape
     :type character: str, required
     :return: HTML entity for the given character
     :rtype: str
     """
     try:
         # Convert character to HTML entity
         return "&#" + str(ord(character)) + ";"
     except TypeError: return ""
 
+def replace_entities(string:str=None) -> str:
+    """
+    Replaces all HTML entities in a string with Unicode characters.
+
+    :param string: Given string
+    :type string: str, required
+    :return: String with HTML escape characters replaced
+    :rtype: str
+    """
+    return regex.regex_replace(entity_to_character, "&[^&;]+;", string)
+
 def replace_reserved_characters(string:str, escape_non_ascii:bool=False) -> str:
     """
     Replaces all reserved HTML characters with escape entities.
     Also replaces all non-ASCII characters, if specified.
 
     :param string: String to replace characters within
     :type string: str, required
     :param escape_non_ascii: Whether to replace non-ASCII characters, defaults to False
     :type escape_non_ascii: bool, optional
     :return: String with reserved characters replaced
     :rtype: str
     """
-    regex = "[<>/='\"&;]"
-    if escape_non_ascii: regex = "[<>/='\"&;]|[^ -~]"
-    return regex_replace(character_to_entity, regex, string)
-
+    regex_string = "[<>/='\"&;]"
+    if escape_non_ascii: regex_string = "[<>/='\"&;]|[^ -~]"
+    return regex.regex_replace(character_to_entity, regex_string, string)
+    
 def replace_reserved_in_html(html_string:str, escape_non_ascii:bool=False) -> str:
     """
     Replaces reserved HTML characters in text which already contains HTML syntax.
     Preserves any text within HTML elements.
 
     :param html_string: HTML string to replace characters within
     :type html_string: str, required
     :param escape_non_ascii: Whether to replace non-ASCII characters, defaults to False
     :type escape_non_ascii: bool, optional
     :return: HTML string with characters replaced with character entities
     :rtype: str
     """
     try:
         # Find all HTML element blocks
-        elements = re_find("<[^<>]+>", html_string)
+        elements = re.findall("<[^<>]+>", html_string)
         # Run through each HTML element
         left_text = html_string
         new_text = ""
         for element in elements:
             # Replace characters in text before the element
             index = left_text.find(element)
             replaced = replace_entities(left_text[:index])
             replaced = replace_reserved_characters(replaced, escape_non_ascii)
             left_text = left_text[index+len(element):]
             new_text = new_text + replaced + element
         # Replace characters in all remaining text
         replaced = replace_entities(left_text)
         new_text = new_text + replace_reserved_characters(replaced, escape_non_ascii)
         return new_text
-    except TypeError: return html_string
+    except TypeError: return html_string
```

## Comparing `html_string_tools/test/test_html_string_tools.py` & `html_string_tools/tests/test_html.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,119 @@
 #!/usr/bin/env
 
-from html_string_tools.main.html_string_tools import character_to_entity
-from html_string_tools.main.html_string_tools import get_extension
-from html_string_tools.main.html_string_tools import entity_to_character
-from html_string_tools.main.html_string_tools import regex_replace
-from html_string_tools.main.html_string_tools import remove_whitespace
-from html_string_tools.main.html_string_tools import replace_entities
-from html_string_tools.main.html_string_tools import replace_reserved_characters as rrc
-from html_string_tools.main.html_string_tools import replace_reserved_in_html as rrih
-
-def test_remove_whitespace():
-    """
-    Tests the remove_whitespace function.
-    """
-    # Test removing whitespace from the beginning and end of strings
-    assert remove_whitespace("") == ""
-    assert remove_whitespace(" ") == ""
-    assert remove_whitespace(" \t  ") == ""
-    assert remove_whitespace("  blah") == "blah"
-    assert remove_whitespace("blah   ") == "blah"
-    assert remove_whitespace(" \t blah  \t") == "blah"
-    assert remove_whitespace(" Other Text \n") == "Other Text"
-    assert remove_whitespace("   Yet \n more Text \n \r") == "Yet \n more Text"    
-    assert remove_whitespace("blah") == "blah"
-    # Test using invalid string
-    assert remove_whitespace(None) is None
-    assert remove_whitespace(4) == 4
+from html_string_tools import html
 
 def test_get_extension():
     """
     Tests the get_extension function.
     """
     # Test getting extensions from filenames
-    assert get_extension("test.png") == ".png"
-    assert get_extension(".long") == ".long"
-    assert get_extension("test2.thing") == ".thing"
-    assert get_extension("blah.test.png") == ".png"
+    assert html.get_extension("test.png") == ".png"
+    assert html.get_extension(".long") == ".long"
+    assert html.get_extension("test2.thing") == ".thing"
+    assert html.get_extension("blah.test.png") == ".png"
     # Test getting extensions from URLs with tokens
-    assert get_extension("test.mp4?extra_.thing") == ".mp4"
-    assert get_extension("thing.test.thing?") == ".thing"
-    assert get_extension("another.txt? test.png?extra.thing") == ".png"
+    assert html.get_extension("test.mp4?extra_.thing") == ".mp4"
+    assert html.get_extension("thing.test.thing?") == ".thing"
+    assert html.get_extension("another.txt? test.png?extra.thing") == ".png"
     # Test getting invalid extensions
-    assert get_extension("test.tolong") == ""
-    assert get_extension("test.notextension") == ""
-    assert get_extension("asdfasdfasdfasdf") == ""
-    assert get_extension("test.tolong?extra") == ""
-    assert get_extension("none?") == ""
+    assert html.get_extension("test.tolong") == ""
+    assert html.get_extension("test.notextension") == ""
+    assert html.get_extension("asdfasdfasdfasdf") == ""
+    assert html.get_extension("test.tolong?extra") == ""
+    assert html.get_extension("none?") == ""
     # Test getting extension if given string is None
-    assert get_extension(None) == ""
-
-def test_regex_replace():
-    """
-    Tests the regex replace function.
-    """
-    # Test replacing regex matches
-    replaced = regex_replace(get_extension, "[a-z]+\\.[a-z]+", "eh, bl.ah th.ing not")
-    assert replaced == "eh, .ah .ing not"
-    replaced = regex_replace(remove_whitespace, "\\s*[0-9]+\\s*", "   Some random  2   text!  1234!  and rest ")
-    assert replaced == "   Some random2text!1234!  and rest "
-    # Test replacing strings with no regex match
-    replaced = regex_replace(get_extension, "nope", "got nothing")
-    assert replaced == "got nothing"
-    # Test replacing strings with invalid parameters
-    assert regex_replace(None, "pattern", "string") == "string"
-    assert regex_replace(get_extension, None, "string") == "string"
-    assert regex_replace(get_extension, "pattern", None) is None
+    assert html.get_extension(None) == ""
 
 def test_entity_to_char():
     """
     Tests the entity_to_char function.
     """
     # Test replacing HTML character entities
-    assert entity_to_character("&quot;") == "\""
-    assert entity_to_character("&apos;") == "'"
-    assert entity_to_character("&amp;") == "&"
-    assert entity_to_character("&lt;") == "<"
-    assert entity_to_character("&gt;") == ">"
-    assert entity_to_character("&nbsp;") == " "
-    assert entity_to_character("&#60;") == "<"
-    assert entity_to_character("&#38;") == "&"
+    assert html.entity_to_character("&quot;") == "\""
+    assert html.entity_to_character("&apos;") == "'"
+    assert html.entity_to_character("&amp;") == "&"
+    assert html.entity_to_character("&lt;") == "<"
+    assert html.entity_to_character("&gt;") == ">"
+    assert html.entity_to_character("&nbsp;") == " "
+    assert html.entity_to_character("&#60;") == "<"
+    assert html.entity_to_character("&#38;") == "&"
     # Test non-latin HTML entities
-    assert entity_to_character("&Agrave;") == "À"
-    assert entity_to_character("&Aacute;") == "Á"
-    assert entity_to_character("&Auml;") == "Ä"
-    assert entity_to_character("&Atilde;") == "Ã"
-    assert entity_to_character("&Aring;") == "Å"
+    assert html.entity_to_character("&Agrave;") == "À"
+    assert html.entity_to_character("&Aacute;") == "Á"
+    assert html.entity_to_character("&Auml;") == "Ä"
+    assert html.entity_to_character("&Atilde;") == "Ã"
+    assert html.entity_to_character("&Aring;") == "Å"
     # Test replacing invalid escape characters
-    assert entity_to_character(None) is None
-    assert entity_to_character("") == ""
-    assert entity_to_character(" ") == " "
-    assert entity_to_character("&;") == "&;"
-    assert entity_to_character("&nope;") == "&nope;"
-    assert entity_to_character("&#nope;") == "&#nope;"
-    assert entity_to_character("&#;") == "&#;"
+    assert html.entity_to_character(None) is None
+    assert html.entity_to_character("") == ""
+    assert html.entity_to_character(" ") == " "
+    assert html.entity_to_character("&;") == "&;"
+    assert html.entity_to_character("&nope;") == "&nope;"
+    assert html.entity_to_character("&#nope;") == "&#nope;"
+    assert html.entity_to_character("&#;") == "&#;"
 
 def test_replace_entities():
     """
     Tests the replace_entities function.
     """
     # Test replacing HTML enities in string
     in_str = "&lt;i&gt;T&euml;st HTML&#60;&#47;i&#62;"
-    assert replace_entities(in_str) == "<i>Tëst HTML</i>"
+    assert html.replace_entities(in_str) == "<i>Tëst HTML</i>"
     in_str = "this&that"
-    assert replace_entities(in_str) == "this&that"
+    assert html.replace_entities(in_str) == "this&that"
     in_str = "remove&this;"
-    assert replace_entities(in_str) == "remove&this;"
+    assert html.replace_entities(in_str) == "remove&this;"
     # Test replacing HTML entities in ivalid test
-    assert replace_entities(None) == None
+    assert html.replace_entities(None) == None
 
 def test_char_to_entity():
     """
     Tests the char_to_entity function.
     """
     # Test converting characters into html escape characters
-    assert character_to_entity("&") == "&#38;"
-    assert character_to_entity("/") == "&#47;"
-    assert character_to_entity("<") == "&#60;"
+    assert html.character_to_entity("&") == "&#38;"
+    assert html.character_to_entity("/") == "&#47;"
+    assert html.character_to_entity("<") == "&#60;"
     # Test converting strings that are too long
-    assert character_to_entity("string") == ""
-    assert character_to_entity("<>") == ""
+    assert html.character_to_entity("string") == ""
+    assert html.character_to_entity("<>") == ""
     # Test converting invalid characters
-    assert character_to_entity(None) == ""
-    assert character_to_entity("") == ""
+    assert html.character_to_entity(None) == ""
+    assert html.character_to_entity("") == ""
 
 def test_replace_reserved_characters():
     """
     Tests the replace_reserved_characters function.
     """
     # Test replacing reserved characters
-    assert rrc("<bláh~!>") == "&#60;bláh~!&#62;"
-    assert rrc("<a href=\"thíng...\">") == "&#60;a href&#61;&#34;thíng...&#34;&#62;"
-    assert rrc("<ímg src='Heh?'>") == "&#60;ímg src&#61;&#39;Heh?&#39;&#62;"
-    assert rrc("&Éh;") == "&#38;Éh&#59;"
+    assert html.replace_reserved_characters("<bláh~!>") == "&#60;bláh~!&#62;"
+    assert html.replace_reserved_characters("<a href=\"thíng...\">") == "&#60;a href&#61;&#34;thíng...&#34;&#62;"
+    assert html.replace_reserved_characters("<ímg src='Heh?'>") == "&#60;ímg src&#61;&#39;Heh?&#39;&#62;"
+    assert html.replace_reserved_characters("&Éh;") == "&#38;Éh&#59;"
     # Test replacing reserved characters and non-ASCII characters
-    assert rrc("<bláh~!>", True) == "&#60;bl&#225;h~!&#62;"
-    assert rrc("<a href=\"thíng...\">", True) == "&#60;a href&#61;&#34;th&#237;ng...&#34;&#62;"
-    assert rrc("<ímg src='Heh?'>", True) == "&#60;&#237;mg src&#61;&#39;Heh?&#39;&#62;"
-    assert rrc("&Éh;", True) == "&#38;&#201;h&#59;"
+    assert html.replace_reserved_characters("<bláh~!>", True) == "&#60;bl&#225;h~!&#62;"
+    assert html.replace_reserved_characters("<a href=\"thíng...\">", True) == "&#60;a href&#61;&#34;th&#237;ng...&#34;&#62;"
+    assert html.replace_reserved_characters("<ímg src='Heh?'>", True) == "&#60;&#237;mg src&#61;&#39;Heh?&#39;&#62;"
+    assert html.replace_reserved_characters("&Éh;", True) == "&#38;&#201;h&#59;"
     # Test replacting reserved characters in invalid string
-    assert rrc(None) is None
-    assert rrc("") == ""
+    assert html.replace_reserved_characters(None) is None
+    assert html.replace_reserved_characters("") == ""
 
 def test_replace_reserved_in_html():
     """
     Tests the replace_reserved_in_html function.
     """
     # Test that HTML tags are kept intact while the rest of text are preserved.
-    assert rrih("<ímg>Bláh!</ímg>", True) == "<ímg>Bl&#225;h!</ímg>"
-    assert rrih("<a href=\"bleh\">&thing;<\a>") == "<a href=\"bleh\">&#38;thing&#59;<\a>"
+    assert html.replace_reserved_in_html("<ímg>Bláh!</ímg>", True) == "<ímg>Bl&#225;h!</ímg>"
+    assert html.replace_reserved_in_html("<a href=\"bleh\">&thing;<\a>") == "<a href=\"bleh\">&#38;thing&#59;<\a>"
     # Test replacing text with no elements
-    assert rrih(">It's a thing!!<") == "&#62;It&#39;s a thing!!&#60;"
+    assert html.replace_reserved_in_html(">It's a thing!!<") == "&#62;It&#39;s a thing!!&#60;"
     # Test replacing text before and after element
-    assert rrih(";; <&thing!> &!") == "&#59;&#59; <&thing!> &#38;!"
+    assert html.replace_reserved_in_html(";; <&thing!> &!") == "&#59;&#59; <&thing!> &#38;!"
     # Tests that already existing escape characters remain intact
-    assert rrih("<a>Th&#237;ng!!</a>", True) == "<a>Th&#237;ng!!</a>"
-    assert rrih("<a>Th&#237;ng!!</a>") == "<a>Thíng!!</a>"
-    assert rrih("&#59; <&!> &#59;") == "&#59; <&!> &#59;"
+    assert html.replace_reserved_in_html("<a>Th&#237;ng!!</a>", True) == "<a>Th&#237;ng!!</a>"
+    assert html.replace_reserved_in_html("<a>Th&#237;ng!!</a>") == "<a>Thíng!!</a>"
+    assert html.replace_reserved_in_html("&#59; <&!> &#59;") == "&#59; <&!> &#59;"
     # Test replacing characters with invalid text
-    assert rrih(None) == None
-    assert rrih("") == ""
+    assert html.replace_reserved_in_html(None) == None
+    assert html.replace_reserved_in_html("") == ""
```

## Comparing `HTML_String_Tools-0.1.0.dist-info/LICENSE` & `HTML_String_Tools-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `HTML_String_Tools-0.1.0.dist-info/METADATA` & `HTML_String_Tools-0.2.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: HTML-String-Tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple set of scripts for handling and formatting HTML formatted text.
 Home-page: https://github.com/Drakovek/HTML-String-Tools
 Author: Drakovek
 Author-email: DrakovekMail@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HTML String Tools
 
 A simple set of scripts for handling and formatting HTML formatted text.
-
-
```

