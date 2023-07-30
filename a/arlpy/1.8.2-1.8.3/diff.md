# Comparing `tmp/arlpy-1.8.2.tar.gz` & `tmp/arlpy-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlpy-1.8.2.tar", last modified: Fri Feb  3 07:48:56 2023, max compression
+gzip compressed data, was "arlpy-1.8.3.tar", last modified: Sun Jul 30 15:18:00 2023, max compression
```

## Comparing `arlpy-1.8.2.tar` & `arlpy-1.8.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-02-03 07:48:56.538913 arlpy-1.8.2/
--rw-r--r--   0 mandar     (501) staff       (20)     1496 2022-12-18 09:26:58.000000 arlpy-1.8.2/LICENSE
--rw-r--r--   0 mandar     (501) staff       (20)       16 2022-12-18 09:26:58.000000 arlpy-1.8.2/MANIFEST.in
--rw-r--r--   0 mandar     (501) staff       (20)     2336 2023-02-03 07:48:56.538780 arlpy-1.8.2/PKG-INFO
--rw-r--r--   0 mandar     (501) staff       (20)     2033 2022-12-18 09:26:58.000000 arlpy-1.8.2/README.rst
-drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-02-03 07:48:56.537854 arlpy-1.8.2/arlpy/
--rw-r--r--   0 mandar     (501) staff       (20)      512 2022-12-18 09:26:58.000000 arlpy-1.8.2/arlpy/__init__.py
--rw-r--r--   0 mandar     (501) staff       (20)    16726 2023-02-03 07:43:48.000000 arlpy-1.8.2/arlpy/bf.py
--rw-r--r--   0 mandar     (501) staff       (20)    19912 2023-02-03 07:43:56.000000 arlpy-1.8.2/arlpy/comms.py
--rw-r--r--   0 mandar     (501) staff       (20)     2496 2023-02-03 07:40:56.000000 arlpy-1.8.2/arlpy/dtla.py
--rw-r--r--   0 mandar     (501) staff       (20)     7211 2022-12-18 09:26:58.000000 arlpy-1.8.2/arlpy/geo.py
--rw-r--r--   0 mandar     (501) staff       (20)     2644 2023-02-03 07:41:00.000000 arlpy-1.8.2/arlpy/hidaq.py
--rw-r--r--   0 mandar     (501) staff       (20)    31346 2023-02-03 07:44:13.000000 arlpy-1.8.2/arlpy/plot.py
--rw-r--r--   0 mandar     (501) staff       (20)     4652 2022-12-18 09:26:58.000000 arlpy-1.8.2/arlpy/romanis.py
--rw-r--r--   0 mandar     (501) staff       (20)    18739 2023-02-03 07:44:22.000000 arlpy-1.8.2/arlpy/signal.py
--rw-r--r--   0 mandar     (501) staff       (20)     4210 2022-12-18 09:26:58.000000 arlpy-1.8.2/arlpy/stable.py
--rw-r--r--   0 mandar     (501) staff       (20)     7116 2023-02-03 07:44:31.000000 arlpy-1.8.2/arlpy/unet.py
--rw-r--r--   0 mandar     (501) staff       (20)     6255 2023-02-03 07:41:40.000000 arlpy-1.8.2/arlpy/utils.py
--rw-r--r--   0 mandar     (501) staff       (20)    10251 2023-02-03 07:04:18.000000 arlpy-1.8.2/arlpy/uwa.py
--rw-r--r--   0 mandar     (501) staff       (20)    36081 2023-02-03 07:44:41.000000 arlpy-1.8.2/arlpy/uwapm.py
-drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-02-03 07:48:56.538591 arlpy-1.8.2/arlpy.egg-info/
--rw-r--r--   0 mandar     (501) staff       (20)     2336 2023-02-03 07:48:56.000000 arlpy-1.8.2/arlpy.egg-info/PKG-INFO
--rw-r--r--   0 mandar     (501) staff       (20)      390 2023-02-03 07:48:56.000000 arlpy-1.8.2/arlpy.egg-info/SOURCES.txt
--rw-r--r--   0 mandar     (501) staff       (20)        1 2023-02-03 07:48:56.000000 arlpy-1.8.2/arlpy.egg-info/dependency_links.txt
--rw-r--r--   0 mandar     (501) staff       (20)       65 2023-02-03 07:48:56.000000 arlpy-1.8.2/arlpy.egg-info/requires.txt
--rw-r--r--   0 mandar     (501) staff       (20)        6 2023-02-03 07:48:56.000000 arlpy-1.8.2/arlpy.egg-info/top_level.txt
--rw-r--r--   0 mandar     (501) staff       (20)       38 2023-02-03 07:48:56.538968 arlpy-1.8.2/setup.cfg
--rw-r--r--   0 mandar     (501) staff       (20)      623 2023-02-03 07:47:52.000000 arlpy-1.8.2/setup.py
+drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-07-30 15:18:00.158992 arlpy-1.8.3/
+-rw-r--r--   0 mandar     (501) staff       (20)     1496 2022-12-18 09:26:58.000000 arlpy-1.8.3/LICENSE
+-rw-r--r--   0 mandar     (501) staff       (20)       16 2022-12-18 09:26:58.000000 arlpy-1.8.3/MANIFEST.in
+-rw-r--r--   0 mandar     (501) staff       (20)     2221 2023-07-30 15:18:00.158867 arlpy-1.8.3/PKG-INFO
+-rw-r--r--   0 mandar     (501) staff       (20)     1918 2023-07-30 15:00:47.000000 arlpy-1.8.3/README.rst
+drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-07-30 15:18:00.157985 arlpy-1.8.3/arlpy/
+-rw-r--r--   0 mandar     (501) staff       (20)      512 2022-12-18 09:26:58.000000 arlpy-1.8.3/arlpy/__init__.py
+-rw-r--r--   0 mandar     (501) staff       (20)    16726 2023-02-03 07:43:48.000000 arlpy-1.8.3/arlpy/bf.py
+-rw-r--r--   0 mandar     (501) staff       (20)    19912 2023-02-03 07:43:56.000000 arlpy-1.8.3/arlpy/comms.py
+-rw-r--r--   0 mandar     (501) staff       (20)     2496 2023-02-03 07:40:56.000000 arlpy-1.8.3/arlpy/dtla.py
+-rw-r--r--   0 mandar     (501) staff       (20)     7211 2022-12-18 09:26:58.000000 arlpy-1.8.3/arlpy/geo.py
+-rw-r--r--   0 mandar     (501) staff       (20)     2644 2023-02-03 07:41:00.000000 arlpy-1.8.3/arlpy/hidaq.py
+-rw-r--r--   0 mandar     (501) staff       (20)    31333 2023-07-30 15:00:47.000000 arlpy-1.8.3/arlpy/plot.py
+-rw-r--r--   0 mandar     (501) staff       (20)     4652 2022-12-18 09:26:58.000000 arlpy-1.8.3/arlpy/romanis.py
+-rw-r--r--   0 mandar     (501) staff       (20)    18739 2023-02-03 07:44:22.000000 arlpy-1.8.3/arlpy/signal.py
+-rw-r--r--   0 mandar     (501) staff       (20)     4210 2022-12-18 09:26:58.000000 arlpy-1.8.3/arlpy/stable.py
+-rw-r--r--   0 mandar     (501) staff       (20)     7116 2023-02-03 07:44:31.000000 arlpy-1.8.3/arlpy/unet.py
+-rw-r--r--   0 mandar     (501) staff       (20)     6255 2023-02-03 07:41:40.000000 arlpy-1.8.3/arlpy/utils.py
+-rw-r--r--   0 mandar     (501) staff       (20)    10251 2023-02-03 07:04:18.000000 arlpy-1.8.3/arlpy/uwa.py
+-rw-r--r--   0 mandar     (501) staff       (20)    36608 2023-07-30 15:00:47.000000 arlpy-1.8.3/arlpy/uwapm.py
+drwxr-xr-x   0 mandar     (501) staff       (20)        0 2023-07-30 15:18:00.158677 arlpy-1.8.3/arlpy.egg-info/
+-rw-r--r--   0 mandar     (501) staff       (20)     2221 2023-07-30 15:18:00.000000 arlpy-1.8.3/arlpy.egg-info/PKG-INFO
+-rw-r--r--   0 mandar     (501) staff       (20)      390 2023-07-30 15:18:00.000000 arlpy-1.8.3/arlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mandar     (501) staff       (20)        1 2023-07-30 15:18:00.000000 arlpy-1.8.3/arlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mandar     (501) staff       (20)       65 2023-07-30 15:18:00.000000 arlpy-1.8.3/arlpy.egg-info/requires.txt
+-rw-r--r--   0 mandar     (501) staff       (20)        6 2023-07-30 15:18:00.000000 arlpy-1.8.3/arlpy.egg-info/top_level.txt
+-rw-r--r--   0 mandar     (501) staff       (20)       38 2023-07-30 15:18:00.159041 arlpy-1.8.3/setup.cfg
+-rw-r--r--   0 mandar     (501) staff       (20)      623 2023-07-30 15:02:37.000000 arlpy-1.8.3/setup.py
```

### Comparing `arlpy-1.8.2/LICENSE` & `arlpy-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/PKG-INFO` & `arlpy-1.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: arlpy
-Version: 1.8.2
+Version: 1.8.3
 Summary: ARL Python Tools
 Home-page: https://github.com/org-arl/arlpy
 Author: Mandar Chitre
 Author-email: mandar@nus.edu.sg
 License: BSD (3-clause)
 Keywords: underwater acoustics signal processing communication
 Platform: UNKNOWN
 License-File: LICENSE
 
-.. image:: https://travis-ci.org/org-arl/arlpy.svg?branch=master
-    :target: https://travis-ci.org/org-arl/arlpy
-
 ARL Python Tools
 ================
 
 Packages such as `numpy` and `scipy` provide excellent mathematical tools for
 scientists and engineers using Python. However, these packages are still young
 and evolving, and understandably have some gaps, especially when it comes to
 domain-specific requirements. The `arlpy` package aims to fill in some of the
```

### Comparing `arlpy-1.8.2/README.rst` & `arlpy-1.8.3/arlpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-.. image:: https://travis-ci.org/org-arl/arlpy.svg?branch=master
-    :target: https://travis-ci.org/org-arl/arlpy
+Metadata-Version: 2.1
+Name: arlpy
+Version: 1.8.3
+Summary: ARL Python Tools
+Home-page: https://github.com/org-arl/arlpy
+Author: Mandar Chitre
+Author-email: mandar@nus.edu.sg
+License: BSD (3-clause)
+Keywords: underwater acoustics signal processing communication
+Platform: UNKNOWN
+License-File: LICENSE
 
 ARL Python Tools
 ================
 
 Packages such as `numpy` and `scipy` provide excellent mathematical tools for
 scientists and engineers using Python. However, these packages are still young
 and evolving, and understandably have some gaps, especially when it comes to
@@ -58,7 +67,9 @@
 for png export. These should be installed manually, if desired.
 
 Useful links
 ------------
 
     * `arlpy home <https://github.com/org-arl/arlpy>`_
     * `arlpy documentation <http://arlpy.readthedocs.io>`_
+
+
```

### Comparing `arlpy-1.8.2/arlpy/__init__.py` & `arlpy-1.8.3/arlpy/__init__.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/bf.py` & `arlpy-1.8.3/arlpy/bf.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/comms.py` & `arlpy-1.8.3/arlpy/comms.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/dtla.py` & `arlpy-1.8.3/arlpy/dtla.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/geo.py` & `arlpy-1.8.3/arlpy/geo.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/hidaq.py` & `arlpy-1.8.3/arlpy/hidaq.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/plot.py` & `arlpy-1.8.3/arlpy/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         height = _figsize[1]
     _color = 0
     tools = []
     if interactive is None:
         interactive = _interactive
     if interactive:
         tools = 'pan,box_zoom,wheel_zoom,reset,save'
-    f = _bplt.figure(title=title, plot_width=width, plot_height=height, x_range=xlim, y_range=ylim, x_axis_label=xlabel, y_axis_label=ylabel, x_axis_type=xtype, y_axis_type=ytype, tools=tools)
+    f = _bplt.figure(title=title, width=width, height=height, x_range=xlim, y_range=ylim, x_axis_label=xlabel, y_axis_label=ylabel, x_axis_type=xtype, y_axis_type=ytype, tools=tools)
     f.toolbar.logo = None
     return f
 
 def _process_canvas(figures):
     global _using_js
     if _disable_js:
         return
@@ -654,15 +654,15 @@
     """
     f, t, Sxx = _sig.spectrogram(x, fs=fs, nperseg=nfft, noverlap=noverlap)
     Sxx = 10*_np.log10(Sxx+_np.finfo(float).eps)
     if isinstance(clim, float) or isinstance(clim, int):
         clim = (_np.max(Sxx)-clim, _np.max(Sxx))
     image(Sxx, x=(t[0], t[-1]), y=(f[0], f[-1]), title=title, colormap=colormap, clim=clim, clabel=clabel, xlabel=xlabel, ylabel=ylabel, xlim=xlim, ylim=ylim, width=width, height=height, hold=hold, interactive=interactive)
 
-def psd(x, fs=2, nfft=512, noverlap=None, window='hanning', color=None, style='solid', thickness=1, marker=None, filled=False, size=6, title=None, xlabel='Frequency (Hz)', ylabel='Power spectral density (dB/Hz)', xlim=None, ylim=None, width=None, height=None, legend=None, hold=False, interactive=None):
+def psd(x, fs=2, nfft=512, noverlap=None, window='hann', color=None, style='solid', thickness=1, marker=None, filled=False, size=6, title=None, xlabel='Frequency (Hz)', ylabel='Power spectral density (dB/Hz)', xlim=None, ylim=None, width=None, height=None, legend=None, hold=False, interactive=None):
     """Plot power spectral density of a given time series signal.
 
     :param x: time series signal
     :param fs: sampling rate
     :param nfft: segment size (see `scipy.signal.welch <https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.welch.html>`_)
     :param noverlap: overlap size (see `scipy.signal.welch`_)
     :param window: window to use (see `scipy.signal.welch`_)
```

### Comparing `arlpy-1.8.2/arlpy/romanis.py` & `arlpy-1.8.3/arlpy/romanis.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/signal.py` & `arlpy-1.8.3/arlpy/signal.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/stable.py` & `arlpy-1.8.3/arlpy/stable.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/unet.py` & `arlpy-1.8.3/arlpy/unet.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/utils.py` & `arlpy-1.8.3/arlpy/utils.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/uwa.py` & `arlpy-1.8.3/arlpy/uwa.py`

 * *Files identical despite different names*

### Comparing `arlpy-1.8.2/arlpy/uwapm.py` & `arlpy-1.8.3/arlpy/uwapm.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,15 +620,17 @@
             self._unlink(fname_base+'.arr')
             self._unlink(fname_base+'.ray')
             self._unlink(fname_base+'.shd')
         return results
 
     def _bellhop(self, *args):
         try:
-            _proc.call(['bellhop.exe'] + list(args), stderr=_proc.STDOUT)
+            _proc.run(f'bellhop.exe {" ".join(list(args))}', 
+                      stderr=_proc.STDOUT, stdout=_proc.PIPE,
+                      shell=True)
         except OSError:
             return False
         return True
 
     def _unlink(self, f):
         try:
             _os.unlink(f)
@@ -651,26 +653,29 @@
     def _create_env_file(self, env, taskcode):
         fh, fname = _mkstemp(suffix='.env')
         fname_base = fname[:-4]
         self._print(fh, "'"+env['name']+"'")
         self._print(fh, "%0.6f" % (env['frequency']))
         self._print(fh, "1")
         svp = env['soundspeed']
+        svp_depth = 0.0
         svp_interp = 'S' if env['soundspeed_interp'] == spline else 'C'
         if isinstance(svp, _pd.DataFrame):
+            svp_depth = svp.index[-1]
             if len(svp.columns) > 1:
                 svp_interp = 'Q'
             else:
                 svp = _np.hstack((_np.array([svp.index]).T, _np.asarray(svp)))
         if env['surface'] is None:
             self._print(fh, "'%cVWT'" % svp_interp)
         else:
             self._print(fh, "'%cVWT*'" % svp_interp)
             self._create_bty_ati_file(fname_base+'.ati', env['surface'], env['surface_interp'])
-        max_depth = env['depth'] if _np.size(env['depth']) == 1 else _np.max(env['depth'][:,1])
+        #max depth should be the depth of the acoustic domain, which can be deeper than the max depth bathymetry
+        max_depth = env['depth'] if _np.size(env['depth']) == 1 else max(_np.max(env['depth'][:,1]), svp_depth)
         self._print(fh, "1 0.0 %0.6f" % (max_depth))
         if _np.size(svp) == 1:
             self._print(fh, "0.0 %0.6f /" % (svp))
             self._print(fh, "%0.6f %0.6f /" % (max_depth, svp))
         elif svp_interp == 'Q':
             for j in range(svp.shape[0]):
                 self._print(fh, "%0.6f %0.6f /" % (svp.index[j], svp.iloc[j,0]))
@@ -780,16 +785,18 @@
                                 'tx_depth_ndx': [j],
                                 'rx_depth_ndx': [k],
                                 'rx_range_ndx': [m],
                                 'tx_depth': [tx_depth[j]],
                                 'rx_depth': [rx_depth[k]],
                                 'rx_range': [rx_range[m]],
                                 'arrival_number': [n],
-                                'arrival_amplitude': [data[0]*_np.exp(1j*data[1])],
+                                # 'arrival_amplitude': [data[0]*_np.exp(1j * data[1]* _np.pi/180)],
+                                'arrival_amplitude': [data[0] * _np.exp( -1j * (_np.deg2rad(data[1]) + freq * 2 * _np.pi * (data[3] * 1j +  data[2])))],
                                 'time_of_arrival': [data[2]],
+                                'complex_time_of_arrival': [data[2] + 1j*data[3]],
                                 'angle_of_departure': [data[4]],
                                 'angle_of_arrival': [data[5]],
                                 'surface_bounces': [data[6]],
                                 'bottom_bounces': [data[7]]
                             }, index=[len(arrivals)+1]))
         return _pd.concat(arrivals)
```

### Comparing `arlpy-1.8.2/arlpy.egg-info/PKG-INFO` & `arlpy-1.8.3/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: arlpy
-Version: 1.8.2
-Summary: ARL Python Tools
-Home-page: https://github.com/org-arl/arlpy
-Author: Mandar Chitre
-Author-email: mandar@nus.edu.sg
-License: BSD (3-clause)
-Keywords: underwater acoustics signal processing communication
-Platform: UNKNOWN
-License-File: LICENSE
-
-.. image:: https://travis-ci.org/org-arl/arlpy.svg?branch=master
-    :target: https://travis-ci.org/org-arl/arlpy
-
 ARL Python Tools
 ================
 
 Packages such as `numpy` and `scipy` provide excellent mathematical tools for
 scientists and engineers using Python. However, these packages are still young
 and evolving, and understandably have some gaps, especially when it comes to
 domain-specific requirements. The `arlpy` package aims to fill in some of the
@@ -70,9 +55,7 @@
 for png export. These should be installed manually, if desired.
 
 Useful links
 ------------
 
     * `arlpy home <https://github.com/org-arl/arlpy>`_
     * `arlpy documentation <http://arlpy.readthedocs.io>`_
-
-
```

### Comparing `arlpy-1.8.2/setup.py` & `arlpy-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     readme = f.read()
 
 setup(
     name='arlpy',
-    version='1.8.2',
+    version='1.8.3',
     description='ARL Python Tools',
     long_description=readme,
     author='Mandar Chitre',
     author_email='mandar@nus.edu.sg',
     url='https://github.com/org-arl/arlpy',
     license='BSD (3-clause)',
     keywords='underwater acoustics signal processing communication',
```

