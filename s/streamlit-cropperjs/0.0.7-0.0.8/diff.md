# Comparing `tmp/streamlit-cropperjs-0.0.7.tar.gz` & `tmp/streamlit-cropperjs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-cropperjs-0.0.7.tar", last modified: Tue Jul 18 12:38:12 2023, max compression
+gzip compressed data, was "streamlit-cropperjs-0.0.8.tar", last modified: Sun Jul 30 04:15:22 2023, max compression
```

## Comparing `streamlit-cropperjs-0.0.7.tar` & `streamlit-cropperjs-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.808768 streamlit-cropperjs-0.0.7/
--rw-rw-rw-   0        0        0     1048 2023-07-15 10:05:27.000000 streamlit-cropperjs-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       55 2023-07-16 08:33:37.000000 streamlit-cropperjs-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1338 2023-07-18 12:38:12.807768 streamlit-cropperjs-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-07-16 09:17:05.000000 streamlit-cropperjs-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 12:38:12.808768 streamlit-cropperjs-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-18 12:37:29.000000 streamlit-cropperjs-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.773247 streamlit-cropperjs-0.0.7/streamlit_cropperjs/
--rw-rw-rw-   0        0        0     4370 2023-07-18 11:27:11.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.765244 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.799767 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/
--rw-rw-rw-   0        0        0      221 2023-07-18 11:30:33.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   197459 2023-07-06 20:11:26.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      471 2023-07-18 11:30:33.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.766244 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.804769 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/
--rw-rw-rw-   0        0        0   291818 2023-07-18 11:30:33.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js
--rw-rw-rw-   0        0        0      881 2023-07-18 11:30:33.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1223450 2023-07-18 11:30:33.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.map
-drwxrwxrwx   0        0        0        0 2023-07-18 12:38:12.795256 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/
--rw-rw-rw-   0        0        0     1338 2023-07-18 12:38:12.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2023-07-18 12:38:12.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:38:12.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 12:38:12.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 12:38:12.000000 streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.703519 streamlit-cropperjs-0.0.8/
+-rw-rw-rw-   0        0        0     1048 2023-07-15 10:05:27.000000 streamlit-cropperjs-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-07-16 08:33:37.000000 streamlit-cropperjs-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1449 2023-07-30 04:15:22.702522 streamlit-cropperjs-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-07-30 04:14:46.000000 streamlit-cropperjs-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 04:15:22.703519 streamlit-cropperjs-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-07-30 04:09:20.000000 streamlit-cropperjs-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.674519 streamlit-cropperjs-0.0.8/streamlit_cropperjs/
+-rw-rw-rw-   0        0        0     4185 2023-07-30 04:14:57.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.667518 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.693521 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/
+-rw-rw-rw-   0        0        0      221 2023-07-30 04:15:16.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   197459 2023-07-06 20:11:26.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      471 2023-07-30 04:15:16.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.668523 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.699520 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   291818 2023-07-30 04:15:16.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js
+-rw-rw-rw-   0        0        0      881 2023-07-30 04:15:16.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1223450 2023-07-30 04:15:16.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.map
+drwxrwxrwx   0        0        0        0 2023-07-30 04:15:22.689518 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/
+-rw-rw-rw-   0        0        0     1449 2023-07-30 04:15:22.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2023-07-30 04:15:22.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 04:15:22.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 04:15:22.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-30 04:15:22.000000 streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/top_level.txt
```

### Comparing `streamlit-cropperjs-0.0.7/LICENSE` & `streamlit-cropperjs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.7/PKG-INFO` & `streamlit-cropperjs-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cropperjs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A streamlit module integrating cropperjs
 Home-page: https://github.com/erjieyong/streamlit-cropperjs
 Author: erjieyong
 Author-email: erjieyong@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,17 @@
 # Streamlit-cropperjs
 
 Integrating the amazing [cropperjs](https://github.com/fengyuanchen/cropperjs) with streamlit. 
 
 This streamlit module is primarily built with mobile usage in mind.
 
 ![](https://github.com/erjieyong/streamlit-cropperjs/blob/main/streamlit-cropperjs-demo.gif)
+## Demo
+Access the demo app here: [https://st-cropperjs.streamlit.app/](https://st-cropperjs.streamlit.app/)
+
 ## Installation
 `pip install streamlit-cropperjs`
 
 ## Example
 ```
 import streamlit as st
 
@@ -28,15 +31,14 @@
 pic = st.file_uploader("Upload a picture", key="uploaded_pic")
 if pic:
     pic = pic.read()
     cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
     if cropped_pic:
         st.image(cropped_pic, output_format="PNG")
 ```
-
 ## Features
 - Crop and return image data
 - Supports touch (mobile)
 - Supports cropping on demand with a button (customised button text)
 
 ## Future Development
 - Support for all cropperjs options
```

### Comparing `streamlit-cropperjs-0.0.7/README.md` & `streamlit-cropperjs-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Streamlit-cropperjs
 
 Integrating the amazing [cropperjs](https://github.com/fengyuanchen/cropperjs) with streamlit. 
 
 This streamlit module is primarily built with mobile usage in mind.
 
 ![](https://github.com/erjieyong/streamlit-cropperjs/blob/main/streamlit-cropperjs-demo.gif)
+## Demo
+Access the demo app here: [https://st-cropperjs.streamlit.app/](https://st-cropperjs.streamlit.app/)
+
 ## Installation
 `pip install streamlit-cropperjs`
 
 ## Example
 ```
 import streamlit as st
 
@@ -17,15 +20,14 @@
 pic = st.file_uploader("Upload a picture", key="uploaded_pic")
 if pic:
     pic = pic.read()
     cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
     if cropped_pic:
         st.image(cropped_pic, output_format="PNG")
 ```
-
 ## Features
 - Crop and return image data
 - Supports touch (mobile)
 - Supports cropping on demand with a button (customised button text)
 
 ## Future Development
 - Support for all cropperjs options
```

### Comparing `streamlit-cropperjs-0.0.7/setup.py` & `streamlit-cropperjs-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-cropperjs",
-    version="0.0.7",
+    version="0.0.8",
     author="erjieyong",
     author_email="erjieyong@gmail.com",
     description="A streamlit module integrating cropperjs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erjieyong/streamlit-cropperjs",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs/__init__.py` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import base64
 import os
+from io import BytesIO
 
 import streamlit as st
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
@@ -46,56 +48,55 @@
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 def st_cropperjs(pic, btn_text, key=None):
     """Create a new instance of "st_cropperjs".
 
     Parameters
     ----------
-    name: str
-        The name of the thing we're saying hello to. The component will display
-        the text "Hello, {name}!"
+    pic: bytes
+        The image file that you want to crop. It should be in bytes format
+    btn_text: str
+        A custom name for the crop button
     key: str or None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
 
     Returns
     -------
-    int
-        The number of times the component's "Click Me" button has been clicked.
-        (This is the value passed to `Streamlit.setComponentValue` on the
-        frontend.)
+    bytes
+        The cropped image file in bytes format
 
     """
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
-    component_value = _st_cropperjs(pic=pic, btn_text=btn_text, key=key, default=None)
+    # cropped_pic is returned as a base64 image in string format
+    cropped_pic = _st_cropperjs(pic=pic, btn_text=btn_text, key=key, default=None)
 
-    # We could modify the value returned from the component if we wanted.
-    # There's no need to do this in our simple example - but it's an option.
-    return component_value
+    if cropped_pic:
+        cropped_pic_base64 = base64.b64decode(
+            cropped_pic.split("data:image/png;base64,")[1]
+        )
+
+        cropped_pic_bytes = BytesIO(cropped_pic_base64).getvalue()
+
+        return cropped_pic_bytes
 
 
 # Add some test code to play with the component while it's in development.
 # During development, we can run this just as we would any other Streamlit
 # app: `$ streamlit run st_cropperjs/__init__.py`
 if not _RELEASE:
     st.subheader("Streamlit-Cropperjs")
     pic = st.file_uploader("Upload a picture", key="uploaded_pic")
     if pic:
         pic = pic.read()
         cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
         if cropped_pic:
             st.image(cropped_pic, output_format="PNG")
-else:
-    st.title("Streamlit-Cropperjs")
-    st.write("Integrating cropperjs by fengyuanchen with streamlit")
-    pic = st.file_uploader("Upload a picture", key="uploaded_pic")
-    if pic:
-        pic = pic.read()
-        cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
-        if cropped_pic:
-            st.image(cropped_pic, output_format="PNG")
+            st.download_button(
+                "Download", cropped_pic, file_name="output.png", mime="image/png"
+            )
```

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/bootstrap.min.css` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.LICENSE.txt` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.map` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs/frontend/build/static/js/main.e894c804.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/PKG-INFO` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cropperjs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A streamlit module integrating cropperjs
 Home-page: https://github.com/erjieyong/streamlit-cropperjs
 Author: erjieyong
 Author-email: erjieyong@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,17 @@
 # Streamlit-cropperjs
 
 Integrating the amazing [cropperjs](https://github.com/fengyuanchen/cropperjs) with streamlit. 
 
 This streamlit module is primarily built with mobile usage in mind.
 
 ![](https://github.com/erjieyong/streamlit-cropperjs/blob/main/streamlit-cropperjs-demo.gif)
+## Demo
+Access the demo app here: [https://st-cropperjs.streamlit.app/](https://st-cropperjs.streamlit.app/)
+
 ## Installation
 `pip install streamlit-cropperjs`
 
 ## Example
 ```
 import streamlit as st
 
@@ -28,15 +31,14 @@
 pic = st.file_uploader("Upload a picture", key="uploaded_pic")
 if pic:
     pic = pic.read()
     cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
     if cropped_pic:
         st.image(cropped_pic, output_format="PNG")
 ```
-
 ## Features
 - Crop and return image data
 - Supports touch (mobile)
 - Supports cropping on demand with a button (customised button text)
 
 ## Future Development
 - Support for all cropperjs options
```

### Comparing `streamlit-cropperjs-0.0.7/streamlit_cropperjs.egg-info/SOURCES.txt` & `streamlit-cropperjs-0.0.8/streamlit_cropperjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

