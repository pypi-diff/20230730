# Comparing `tmp/dash_deckgl-0.2.1.tar.gz` & `tmp/dash_deckgl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_deckgl-0.2.1.tar", last modified: Mon Jul 24 03:53:47 2023, max compression
+gzip compressed data, was "dash_deckgl-0.2.2.tar", last modified: Sun Jul 30 19:50:16 2023, max compression
```

## Comparing `dash_deckgl-0.2.1.tar` & `dash_deckgl-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.2.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.2.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.2.1/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.792070 dash_deckgl-0.2.1/dash_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2981 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/DashDeckgl.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.2.1/dash_deckgl/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/_imports_.py
--rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-07-24 03:44:21.000000 dash_deckgl-0.2.1/dash_deckgl/dash_deckgl.min.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    16785 2023-07-24 03:44:21.000000 dash_deckgl-0.2.1/dash_deckgl/deckgl.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     2917 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/metadata.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-24 03:38:40.000000 dash_deckgl-0.2.1/dash_deckgl/package-info.json
--rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.2.1/dash_deckgl/vendor.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/dash_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-24 03:34:20.000000 dash_deckgl-0.2.1/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.2.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.2.1/tests/test_usage.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 19:50:16.244363 dash_deckgl-0.2.2/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.2.2/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.2.2/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-30 19:50:16.244363 dash_deckgl-0.2.2/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.2.2/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 19:50:16.240363 dash_deckgl-0.2.2/dash_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3126 2023-07-28 02:55:04.000000 dash_deckgl-0.2.2/dash_deckgl/DashDeckgl.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.2.2/dash_deckgl/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-07-28 02:55:04.000000 dash_deckgl-0.2.2/dash_deckgl/_imports_.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)  1202643 2023-07-28 02:55:02.000000 dash_deckgl-0.2.2/dash_deckgl/dash_deckgl.min.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16762 2023-07-28 02:55:02.000000 dash_deckgl-0.2.2/dash_deckgl/deckgl.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3103 2023-07-28 02:55:04.000000 dash_deckgl-0.2.2/dash_deckgl/metadata.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-28 02:55:03.000000 dash_deckgl-0.2.2/dash_deckgl/package-info.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.2.2/dash_deckgl/vendor.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 19:50:16.244363 dash_deckgl-0.2.2/dash_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-30 19:50:15.000000 dash_deckgl-0.2.2/dash_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-07-30 19:50:16.000000 dash_deckgl-0.2.2/dash_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-30 19:50:15.000000 dash_deckgl-0.2.2/dash_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-07-30 19:50:15.000000 dash_deckgl-0.2.2/dash_deckgl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-28 02:52:10.000000 dash_deckgl-0.2.2/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-30 19:50:16.244363 dash_deckgl-0.2.2/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.2.2/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 19:50:16.244363 dash_deckgl-0.2.2/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.2.2/tests/test_usage.py
```

### Comparing `dash_deckgl-0.2.1/PKG-INFO` & `dash_deckgl-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dash_deckgl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package: dashDeckgl
 Title: Deck.gl component for Dash
-Version: 0.2.1
+Version: 0.2.2
 Description: Deck.gl component for Dash
 Depends: R (>= 3.0.2)
 Imports: 
 Suggests: 
 License: MIT + file LICENSE
 URL: https://github.com/oceanum-io/dash-deckgl
 BugReports: https://github.com/oceanum-io/dash-deckgl/issues
```

### Comparing `dash_deckgl-0.2.1/README.md` & `dash_deckgl-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.1/dash_deckgl/DashDeckgl.py` & `dash_deckgl-0.2.2/dash_deckgl/DashDeckgl.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 - height (number; optional):
     Height of the map component container as pixels or CSS string
     (optional) Default 500.
 
 - lastEvent (dict; optional):
     The last event that was triggered. This is a read-only property.
 
+- mapbox_key (string; optional):
+    mapbox API key for mapbox basemaps (optional).
+
 - overlay (string; optional):
     JSON spec of the overlay deck.gl instance (optional).
 
 - spec (string; required):
     JSON spec of the primary deck.gl instance.
 
 - tooltips (list; optional):
@@ -50,18 +53,18 @@
     width of the map component container as pixels or CSS string
     (optional) Default 100% of parent container."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_deckgl'
     _type = 'DashDeckgl'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, spec=Component.REQUIRED, tooltips=Component.UNDEFINED, width=Component.UNDEFINED, height=Component.UNDEFINED, customLibraries=Component.UNDEFINED, configuration=Component.UNDEFINED, description=Component.UNDEFINED, events=Component.UNDEFINED, overlay=Component.UNDEFINED, lastEvent=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltips', 'width']
+    def __init__(self, id=Component.UNDEFINED, spec=Component.REQUIRED, tooltips=Component.UNDEFINED, width=Component.UNDEFINED, height=Component.UNDEFINED, customLibraries=Component.UNDEFINED, configuration=Component.UNDEFINED, description=Component.UNDEFINED, events=Component.UNDEFINED, overlay=Component.UNDEFINED, mapbox_key=Component.UNDEFINED, lastEvent=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'mapbox_key', 'overlay', 'spec', 'tooltips', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltips', 'width']
+        self.available_properties = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'mapbox_key', 'overlay', 'spec', 'tooltips', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['spec']:
```

### Comparing `dash_deckgl-0.2.1/dash_deckgl/__init__.py` & `dash_deckgl-0.2.2/dash_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.1/dash_deckgl/dash_deckgl.min.js` & `dash_deckgl-0.2.2/dash_deckgl/dash_deckgl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50007,15 +50007,15 @@
         var l = jsonpScriptSrc;
         jsonpScriptSrc = function(t) {
             var e, n = (e = A(), /\/_dash-component-suites\//.test(e.src)),
                 i = l(t);
             if (!n) return i;
             var r = i.split("/"),
                 s = r.slice(-1)[0].split(".");
-            return s.splice(1, 0, "v0_2_1m1690170242"), r.splice(-1, 1, s.join(".")), r.join("/")
+            return s.splice(1, 0, "v0_2_2m1690512881"), r.splice(-1, 1, s.join(".")), r.join("/")
         }
     }(() => {
         var t = {
             179: 0
         };
         o.f.j = (e, n) => {
             var i = o.o(t, e) ? t[e] : void 0;
@@ -50072,14 +50072,15 @@
             width: i().number,
             height: i().number,
             customLibraries: i().array,
             configuration: i().object,
             description: i().object,
             events: i().array,
             overlay: i().string,
+            mapbox_key: i().string,
             setProps: i().func,
             lastEvent: i().object
         };
         const a = s;
         var A = o(4144),
             l = o(8339),
             u = o(4933);
```

### Comparing `dash_deckgl-0.2.1/dash_deckgl/deckgl.js` & `dash_deckgl-0.2.2/dash_deckgl/deckgl.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -388,18 +388,18 @@
                             }))
                         }
                     }), [i]), a().createElement(P.Provider, {
                         value: u
                     }, l)
                 };
 
-            function _(e, r) {
+            function C(e, r) {
                 var t = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                 if (!t) {
-                    if (Array.isArray(e) || (t = C(e)) || r && e && "number" == typeof e.length) {
+                    if (Array.isArray(e) || (t = _(e)) || r && e && "number" == typeof e.length) {
                         t && (e = t);
                         var n = 0,
                             o = function() {};
                         return {
                             s: o,
                             n: function() {
                                 return n >= e.length ? {
@@ -436,54 +436,54 @@
                         } finally {
                             if (l) throw a
                         }
                     }
                 }
             }
 
-            function C(e, r) {
+            function _(e, r) {
                 if (e) {
                     if ("string" == typeof e) return A(e, r);
                     var t = Object.prototype.toString.call(e).slice(8, -1);
                     return "Object" === t && e.constructor && (t = e.constructor.name), "Map" === t || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? A(e, r) : void 0
                 }
             }
 
             function A(e, r) {
                 (null == r || r > e.length) && (r = e.length);
                 for (var t = 0, n = new Array(r); t < r; t++) n[t] = e[t];
                 return n
             }
-            var G = {
+            var j = {
                 fontFamily: '"Helvetica Neue", Helvetica, Arial, sans-serif',
                 display: "flex",
                 flex: "wrap",
                 maxWidth: "500px",
                 flexDirection: "column",
                 zIndex: 2
             };
 
-            function j(e, r) {
+            function G(e, r) {
                 var t, n, o, a = e,
                     i = "properties",
-                    l = _(function(e) {
+                    l = C(function(e) {
                         if (Array.isArray(e)) return A(e)
                     }(o = new Set(e.match(/{[^}]*}/g).map((function(e) {
                         return e.replace(/[{}]/g, "")
                     })))) || function(e) {
                         if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                    }(o) || C(o) || function() {
+                    }(o) || _(o) || function() {
                         throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                     }());
                 try {
                     for (l.s(); !(n = l.n()).done;) {
                         var c = n.value;
                         if (c.includes(".")) {
                             t = r;
-                            var u, s = _(c.split("."));
+                            var u, s = C(c.split("."));
                             try {
                                 for (s.s(); !(u = s.n()).done;) {
                                     var y = u.value;
                                     if (!t.hasOwnProperty(y)) {
                                         t = void 0;
                                         break
                                     }
@@ -618,133 +618,132 @@
                     s = e.height,
                     y = void 0 === s ? 500 : s,
                     f = e.events,
                     p = void 0 === f ? [] : f,
                     m = e.description,
                     g = e.overlay,
                     d = e.mapbox_key,
-                    b = e.google_maps_key,
-                    h = e.setProps,
-                    v = (e.lastEvent, M((0, o.useState)({}), 2)),
-                    L = v[0],
-                    S = v[1],
-                    w = M((0, o.useState)({}), 2),
-                    O = w[0],
-                    T = w[1],
-                    E = M((0, o.useState)(!1), 2),
-                    _ = (E[0], E[1], M((0, o.useState)(!1), 2)),
-                    C = (_[0], _[1], (0, o.useContext)(P)),
-                    A = M((0, o.useState)(null), 2),
-                    x = A[0],
-                    k = A[1],
-                    N = [];
+                    b = e.setProps,
+                    h = (e.lastEvent, M((0, o.useState)({}), 2)),
+                    v = h[0],
+                    L = h[1],
+                    S = M((0, o.useState)({}), 2),
+                    w = S[0],
+                    O = S[1],
+                    T = M((0, o.useState)(!1), 2),
+                    E = (T[0], T[1], M((0, o.useState)(!1), 2)),
+                    C = (E[0], E[1], (0, o.useContext)(P)),
+                    _ = M((0, o.useState)(null), 2),
+                    A = _[0],
+                    x = _[1],
+                    k = [];
                 if (m)
-                    for (var F in m)
-                        if (["top-right", "top-left", "bottom-right", "bottom-left"].includes(F)) {
-                            var R = F.split("-");
-                            N.push({
-                                pos: R,
-                                content: m[F]
+                    for (var N in m)
+                        if (["top-right", "top-left", "bottom-right", "bottom-left"].includes(N)) {
+                            var F = N.split("-");
+                            k.push({
+                                pos: F,
+                                content: m[N]
                             })
-                        } var U = (0, o.useCallback)((function(e, r) {
-                        p.includes(e) && h({
+                        } var R = (0, o.useCallback)((function(e, r) {
+                        p.includes(e) && b({
                             lastEvent: D(D({}, r.object), {}, {
                                 coordinate: r.coordinate,
                                 eventType: e
                             })
                         })
                     }), [p]),
-                    H = {
+                    U = {
                         onClick: function(e) {
-                            return U("click", e)
+                            return R("click", e)
                         },
                         onHover: function(e) {
-                            return U("hover", e)
+                            return R("hover", e)
                         },
                         onDragStart: function(e) {
-                            return U("drag-start", e)
+                            return R("drag-start", e)
                         },
                         onDrag: function(e) {
-                            return U("drag", e)
+                            return R("drag", e)
                         },
                         onDragEnd: function(e) {
-                            return U("drag-end", e)
+                            return R("drag-end", e)
                         }
                     },
-                    B = function(e) {
+                    H = function(e) {
                         return e ? e.length ? function(r) {
                             if (!r.picked) return null;
                             var t = null;
                             return e.map((function(e) {
                                 if (e.layer && r.layer.id != e.layer) return null;
                                 t = {
-                                    style: e.style || G
-                                }, e.html ? t.html = j(e.html, r.object) : t.text = j(e.text, r.object)
+                                    style: e.style || j
+                                }, e.html ? t.html = G(e.html, r.object) : t.text = G(e.text, r.object)
                             })), t
                         } : getTooltipDefault : null
                     }(t),
-                    J = D(D({}, H), {}, {
-                        getTooltip: B
+                    B = D(D({}, U), {}, {
+                        getTooltip: H
                     });
                 (0, o.useEffect)((function() {
                     ! function() {
                         var e, r;
                         e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "https://api.tiles.mapbox.com/mapbox-gl-js/v1.13.2/mapbox-gl.css", (r = document.createElement("link")).type = "text/css", r.rel = "stylesheet", r.href = e, document.getElementsByTagName("head")[0].appendChild(r)
                     }()
                 }), []), (0, o.useEffect)((function() {
                     var e = C.convert(r);
-                    console.log(e), e.initialViewState && k(e.initialViewState), S(D(D({}, L), e))
+                    console.log(e), e.initialViewState && (!A || e.initialViewState.longitude && e.initialViewState.latitude) && x(e.initialViewState), L(D(D({}, v), e))
                 }), [r, C]), (0, o.useEffect)((function() {
                     var e = C.convert(g);
-                    T(D(D({}, O), e))
+                    O(D(D({}, w), e))
                 }), [g, C]);
-                var W = (0, o.useCallback)((function(e) {
+                var J = (0, o.useCallback)((function(e) {
                     var r = e.viewState;
-                    k(r)
+                    x(r)
                 }), []);
-                return b ? a().createElement("div", null, "Google map overlays not supported") : a().createElement("div", {
+                return a().createElement("div", {
                     className: "deckgl-map",
                     style: {
                         height: y,
                         width: u,
                         position: "relative"
                     }
                 }, a().createElement("div", {
                     id: "deckgl-primary",
                     style: {
                         width: "100%",
                         height: "100%",
                         position: "relative"
                     }
-                }, x && a().createElement(i.Z, I({
-                    viewState: x,
-                    onViewStateChange: W
-                }, J, L), a().createElement(c.D5, {
-                    mapStyle: L.mapStyle || l.Z.POSITRON,
+                }, A && a().createElement(i.Z, I({
+                    viewState: A,
+                    onViewStateChange: J
+                }, B, v), a().createElement(c.D5, {
+                    mapStyle: v.mapStyle || l.Z.POSITRON,
                     mapboxAccessToken: d
                 }))), g && a().createElement("div", {
                     id: "deckgl-overlay",
                     style: {
                         width: "100%",
                         height: "100%",
                         position: "relative",
                         pointerEvents: "none"
                     }
                 }, a().createElement(i.Z, I({
-                    viewState: x,
+                    viewState: A,
                     contoller: !1
-                }, J, O, {
-                    style: D(D({}, O.style), {}, {
+                }, B, w, {
+                    style: D(D({}, w.style), {}, {
                         zIndex: 1,
                         pointerEvents: "none"
                     })
                 }), a().createElement(c.D5, {
-                    mapStyle: O.mapStyle,
+                    mapStyle: w.mapStyle,
                     mapboxAccessToken: d
-                }))), N.map((function(e, r) {
+                }))), k.map((function(e, r) {
                     var t;
                     return a().createElement("div", {
                         key: r,
                         className: "description",
                         style: (t = {
                             position: "absolute",
                             zIndex: 10
```

### Comparing `dash_deckgl-0.2.1/dash_deckgl/metadata.json` & `dash_deckgl-0.2.2/dash_deckgl/metadata.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'src/lib/components/DashDeckgl.react.js'": "{'props': {'mapbox_key': OrderedDict([('type', "*

 * *                                             "OrderedDict([('name', 'string')])), ('required', "*

 * *                                             "False), ('description', 'mapbox API key for mapbox "*

 * *                                             "basemaps\\n(optional)')])}}"}*

```diff
@@ -49,14 +49,21 @@
             "lastEvent": {
                 "description": "The last event that was triggered. This is a read-only property.",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
+            "mapbox_key": {
+                "description": "mapbox API key for mapbox basemaps\n(optional)",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
             "overlay": {
                 "description": "JSON spec of the overlay deck.gl instance\n(optional)",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
```

### Comparing `dash_deckgl-0.2.1/dash_deckgl/package-info.json` & `dash_deckgl-0.2.2/dash_deckgl/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `dash_deckgl-0.2.1/dash_deckgl/vendor.js` & `dash_deckgl-0.2.2/dash_deckgl/vendor.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.1/dash_deckgl.egg-info/PKG-INFO` & `dash_deckgl-0.2.2/dash_deckgl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dash-deckgl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package: dashDeckgl
 Title: Deck.gl component for Dash
-Version: 0.2.1
+Version: 0.2.2
 Description: Deck.gl component for Dash
 Depends: R (>= 3.0.2)
 Imports: 
 Suggests: 
 License: MIT + file LICENSE
 URL: https://github.com/oceanum-io/dash-deckgl
 BugReports: https://github.com/oceanum-io/dash-deckgl/issues
```

### Comparing `dash_deckgl-0.2.1/package.json` & `dash_deckgl-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `dash_deckgl-0.2.1/setup.py` & `dash_deckgl-0.2.2/setup.py`

 * *Files identical despite different names*

