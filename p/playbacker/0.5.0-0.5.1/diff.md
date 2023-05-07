# Comparing `tmp/playbacker-0.5.0.tar.gz` & `tmp/playbacker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playbacker-0.5.0.tar", max compression
+gzip compressed data, was "playbacker-0.5.1.tar", max compression
```

## Comparing `playbacker-0.5.0.tar` & `playbacker-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1253 2023-04-03 09:03:59.623265 playbacker-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/__init__.py
--rw-r--r--   0        0        0     5020 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/app.py
--rw-r--r--   0        0        0      527 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/config.py
--rw-r--r--   0        0        0        0 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/__init__.py
--rw-r--r--   0        0        0      850 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/audiofile.py
--rw-r--r--   0        0        0     1292 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/clock.py
--rw-r--r--   0        0        0     3423 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/playback.py
--rw-r--r--   0        0        0     1444 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/player.py
--rw-r--r--   0        0        0      952 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/setlist.py
--rw-r--r--   0        0        0     3408 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/settings.py
--rw-r--r--   0        0        0      892 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/song.py
--rw-r--r--   0        0        0     3137 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/stream.py
--rw-r--r--   0        0        0      757 2023-04-03 09:03:20.534798 playbacker-0.5.0/src/playbacker/core/tempo.py
--rw-r--r--   0        0        0     2607 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/core/track.py
--rw-r--r--   0        0        0        0 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/core/tracks/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/core/tracks/countdown.py
--rw-r--r--   0        0        0     2064 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/core/tracks/metronome.py
--rw-r--r--   0        0        0     1078 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/core/validate.py
--rw-r--r--   0        0        0    22120 2023-04-03 09:03:58.883260 playbacker-0.5.0/src/playbacker/dist/assets/index-1ebba71c.js
--rw-r--r--   0        0        0     8295 2023-04-03 09:03:58.883260 playbacker-0.5.0/src/playbacker/dist/assets/index-c1f1d727.css
--rw-r--r--   0        0        0      388 2023-04-03 09:03:58.883260 playbacker-0.5.0/src/playbacker/dist/index.html
--rw-r--r--   0        0        0     2807 2023-04-03 09:03:20.538798 playbacker-0.5.0/src/playbacker/main.py
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 playbacker-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1254 2023-05-07 01:46:02.339974 playbacker-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/__init__.py
+-rw-r--r--   0        0        0     5020 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/app.py
+-rw-r--r--   0        0        0      527 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/config.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/__init__.py
+-rw-r--r--   0        0        0      850 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/audiofile.py
+-rw-r--r--   0        0        0     1292 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/clock.py
+-rw-r--r--   0        0        0     3423 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/playback.py
+-rw-r--r--   0        0        0     1444 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/player.py
+-rw-r--r--   0        0        0      952 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/setlist.py
+-rw-r--r--   0        0        0     3408 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/settings.py
+-rw-r--r--   0        0        0      892 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/song.py
+-rw-r--r--   0        0        0     3137 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/stream.py
+-rw-r--r--   0        0        0      757 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tempo.py
+-rw-r--r--   0        0        0     2607 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/track.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/__init__.py
+-rw-r--r--   0        0        0     1812 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/countdown.py
+-rw-r--r--   0        0        0     2064 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/metronome.py
+-rw-r--r--   0        0        0     1078 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/validate.py
+-rw-r--r--   0        0        0    21934 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/assets/index-04f532a9.js
+-rw-r--r--   0        0        0     8295 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/assets/index-c1f1d727.css
+-rw-r--r--   0        0        0      388 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/index.html
+-rw-r--r--   0        0        0     2807 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/main.py
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 playbacker-0.5.1/PKG-INFO
```

### Comparing `playbacker-0.5.0/pyproject.toml` & `playbacker-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "playbacker"
-version = "v0.5.0"
+version = "v0.5.1"
 description = "Live music performance playback"
 authors = ["Lev Vereshchagin <mail@vrslev.com>"]
 license = "MIT"
 # TODO: readme
 # readme = "../README.md"
 include = ["src/playbacker/dist/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sounddevice = "0.4.6"
 SoundFile = "0.12.1"
-numpy = "1.24.2"
+numpy = "1.24.3"
 pydantic = "1.10.7"
 PyYAML = "6.0"
 typer = { extras = ["all"], version = "0.7.0" }
 uvloop = "0.17.0"
 inquirer = "3.1.3"
-soxr = "0.3.4"
-starlite = "1.51.9"
+soxr = "0.3.5"
+starlite = "1.51.10"
 uvicorn = { extras = ["standard"], version = "0.21.1" }
 watchfiles = "0.19.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "7.2.1"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
-pyright = "1.1.301"
+pyright = "1.1.304"
 
 [build-system]
 requires = [
     "poetry-core>1.0.7",         # 1.0.8 supports PEP 660 — editable installs
     "poetry-dynamic-versioning",
 ]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `playbacker-0.5.0/src/playbacker/app.py` & `playbacker-0.5.1/src/playbacker/app.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/config.py` & `playbacker-0.5.1/src/playbacker/config.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/audiofile.py` & `playbacker-0.5.1/src/playbacker/core/audiofile.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/clock.py` & `playbacker-0.5.1/src/playbacker/core/clock.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/playback.py` & `playbacker-0.5.1/src/playbacker/core/playback.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/player.py` & `playbacker-0.5.1/src/playbacker/core/player.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/setlist.py` & `playbacker-0.5.1/src/playbacker/core/setlist.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/settings.py` & `playbacker-0.5.1/src/playbacker/core/settings.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/song.py` & `playbacker-0.5.1/src/playbacker/core/song.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/stream.py` & `playbacker-0.5.1/src/playbacker/core/stream.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/tempo.py` & `playbacker-0.5.1/src/playbacker/core/tempo.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/track.py` & `playbacker-0.5.1/src/playbacker/core/track.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/tracks/countdown.py` & `playbacker-0.5.1/src/playbacker/core/tracks/countdown.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/tracks/metronome.py` & `playbacker-0.5.1/src/playbacker/core/tracks/metronome.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/core/validate.py` & `playbacker-0.5.1/src/playbacker/core/validate.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/dist/assets/index-1ebba71c.js` & `playbacker-0.5.1/src/playbacker/dist/assets/index-04f532a9.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,36 @@
 (function() {
     const n = document.createElement("link").relList;
     if (n && n.supports && n.supports("modulepreload")) return;
-    for (const r of document.querySelectorAll('link[rel="modulepreload"]')) l(r);
-    new MutationObserver(r => {
-        for (const i of r)
+    for (const l of document.querySelectorAll('link[rel="modulepreload"]')) r(l);
+    new MutationObserver(l => {
+        for (const i of l)
             if (i.type === "childList")
-                for (const o of i.addedNodes) o.tagName === "LINK" && o.rel === "modulepreload" && l(o)
+                for (const o of i.addedNodes) o.tagName === "LINK" && o.rel === "modulepreload" && r(o)
     }).observe(document, {
         childList: !0,
         subtree: !0
     });
 
-    function t(r) {
+    function t(l) {
         const i = {};
-        return r.integrity && (i.integrity = r.integrity), r.referrerPolicy && (i.referrerPolicy = r.referrerPolicy), r.crossOrigin === "use-credentials" ? i.credentials = "include" : r.crossOrigin === "anonymous" ? i.credentials = "omit" : i.credentials = "same-origin", i
+        return l.integrity && (i.integrity = l.integrity), l.referrerPolicy && (i.referrerPolicy = l.referrerPolicy), l.crossOrigin === "use-credentials" ? i.credentials = "include" : l.crossOrigin === "anonymous" ? i.credentials = "omit" : i.credentials = "same-origin", i
     }
 
-    function l(r) {
-        if (r.ep) return;
-        r.ep = !0;
-        const i = t(r);
-        fetch(r.href, i)
+    function r(l) {
+        if (l.ep) return;
+        l.ep = !0;
+        const i = t(l);
+        fetch(l.href, i)
     }
 })();
-const Se = (e, n) => e === n,
+const pe = (e, n) => e === n,
     Oe = Symbol("solid-track"),
     X = {
-        equals: Se
+        equals: pe
     };
 let Ee = Pe;
 const O = 1,
     Y = 2,
     Ae = {
         owned: null,
         cleanups: null,
@@ -39,170 +39,170 @@
     },
     ie = {};
 var C = null;
 let se = null,
     $ = null,
     A = null,
     V = null,
-    le = 0;
+    re = 0;
 
 function Q(e, n) {
     const t = $,
-        l = C,
-        r = e.length === 0,
-        i = r ? Ae : {
+        r = C,
+        l = e.length === 0,
+        i = l ? Ae : {
             owned: null,
             cleanups: null,
             context: null,
-            owner: n === void 0 ? l : n
+            owner: n === void 0 ? r : n
         },
-        o = r ? e : () => e(() => I(() => re(i)));
+        o = l ? e : () => e(() => I(() => le(i)));
     C = i, $ = null;
     try {
         return j(o, !0)
     } finally {
-        $ = t, C = l
+        $ = t, C = r
     }
 }
 
 function M(e, n) {
     n = n ? Object.assign({}, X, n) : X;
     const t = {
             value: e,
             observers: null,
             observerSlots: null,
             comparator: n.equals || void 0
         },
-        l = r => (typeof r == "function" && (r = r(t.value)), Ne(t, r));
-    return [Ce.bind(t), l]
+        r = l => (typeof l == "function" && (l = l(t.value)), Ne(t, l));
+    return [Ce.bind(t), r]
 }
 
 function de(e, n, t) {
-    const l = W(e, n, !0, O);
-    R(l)
+    const r = W(e, n, !0, O);
+    R(r)
 }
 
 function H(e, n, t) {
-    const l = W(e, n, !1, O);
-    R(l)
+    const r = W(e, n, !1, O);
+    R(r)
 }
 
 function J(e, n, t) {
     Ee = Ue;
-    const l = W(e, n, !1, O);
-    l.user = !0, V ? V.push(l) : R(l)
+    const r = W(e, n, !1, O);
+    (!t || !t.render) && (r.user = !0), V ? V.push(r) : R(r)
 }
 
 function Z(e, n, t) {
     t = t ? Object.assign({}, X, t) : X;
-    const l = W(e, n, !0, 0);
-    return l.observers = null, l.observerSlots = null, l.comparator = t.equals || void 0, R(l), Ce.bind(l)
+    const r = W(e, n, !0, 0);
+    return r.observers = null, r.observerSlots = null, r.comparator = t.equals || void 0, R(r), Ce.bind(r)
 }
 
 function ge(e, n, t) {
-    let l, r, i;
-    arguments.length === 2 && typeof n == "object" || arguments.length === 1 ? (l = !0, r = e, i = n || {}) : (l = e, r = n, i = t || {});
+    let r, l, i;
+    arguments.length === 2 && typeof n == "object" || arguments.length === 1 ? (r = !0, l = e, i = n || {}) : (r = e, l = n, i = t || {});
     let o = null,
         s = ie,
         f = !1,
         c = "initialValue" in i,
-        a = typeof l == "function" && Z(l);
+        a = typeof r == "function" && Z(r);
     const m = new Set,
         [u, h] = (i.storage || M)(i.initialValue),
         [d, N] = M(void 0),
         [T, L] = M(void 0, {
             equals: !1
         }),
-        [p, y] = M(c ? "ready" : "unresolved");
+        [_, y] = M(c ? "ready" : "unresolved");
 
-    function w(x, _, S, D) {
-        return o === x && (o = null, c = !0, (x === s || _ === s) && i.onHydrated && queueMicrotask(() => i.onHydrated(D, {
-            value: _
-        })), s = ie, g(_, S)), _
+    function v(x, S, p, D) {
+        return o === x && (o = null, c = !0, (x === s || S === s) && i.onHydrated && queueMicrotask(() => i.onHydrated(D, {
+            value: S
+        })), s = ie, g(S, p)), S
     }
 
-    function g(x, _) {
+    function g(x, S) {
         j(() => {
-            _ === void 0 && h(() => x), y(_ !== void 0 ? "errored" : "ready"), N(_);
-            for (const S of m.keys()) S.decrement();
+            S === void 0 && h(() => x), y(S !== void 0 ? "errored" : "ready"), N(S);
+            for (const p of m.keys()) p.decrement();
             m.clear()
         }, !1)
     }
 
-    function v() {
+    function w() {
         const x = Me,
-            _ = u(),
-            S = d();
-        if (S !== void 0 && !o) throw S;
+            S = u(),
+            p = d();
+        if (p !== void 0 && !o) throw p;
         return $ && !$.user && x && de(() => {
             T(), o && (x.resolved || m.has(x) || (x.increment(), m.add(x)))
-        }), _
+        }), S
     }
 
     function E(x = !0) {
         if (x !== !1 && f) return;
         f = !1;
-        const _ = a ? a() : l;
-        if (_ == null || _ === !1) {
-            w(o, I(u));
+        const S = a ? a() : r;
+        if (S == null || S === !1) {
+            v(o, I(u));
             return
         }
-        const S = s !== ie ? s : I(() => r(_, {
+        const p = s !== ie ? s : I(() => l(S, {
             value: u(),
             refetching: x
         }));
-        return typeof S != "object" || !(S && "then" in S) ? (w(o, S, void 0, _), S) : (o = S, f = !0, queueMicrotask(() => f = !1), j(() => {
+        return typeof p != "object" || !(p && "then" in p) ? (v(o, p, void 0, S), p) : (o = p, f = !0, queueMicrotask(() => f = !1), j(() => {
             y(c ? "refreshing" : "pending"), L()
-        }, !1), S.then(D => w(S, D, void 0, _), D => w(S, void 0, De(D), _)))
+        }, !1), p.then(D => v(p, D, void 0, S), D => v(p, void 0, De(D), S)))
     }
-    return Object.defineProperties(v, {
+    return Object.defineProperties(w, {
         state: {
-            get: () => p()
+            get: () => _()
         },
         error: {
             get: () => d()
         },
         loading: {
             get() {
-                const x = p();
+                const x = _();
                 return x === "pending" || x === "refreshing"
             }
         },
         latest: {
             get() {
-                if (!c) return v();
+                if (!c) return w();
                 const x = d();
                 if (x && !o) throw x;
                 return u()
             }
         }
-    }), a ? de(() => E(!1)) : E(!1), [v, {
+    }), a ? de(() => E(!1)) : E(!1), [w, {
         refetch: E,
         mutate: h
     }]
 }
 
-function he(e, n = Se, t) {
-    const l = new Map,
-        r = W(i => {
+function he(e, n = pe, t) {
+    const r = new Map,
+        l = W(i => {
             const o = e();
-            for (const [s, f] of l.entries())
+            for (const [s, f] of r.entries())
                 if (n(s, o) !== n(s, i))
                     for (const c of f.values()) c.state = O, c.pure ? A.push(c) : V.push(c);
             return o
         }, void 0, !0, O);
-    return R(r), i => {
+    return R(l), i => {
         const o = $;
         if (o) {
             let s;
-            (s = l.get(i)) ? s.add(o): l.set(i, s = new Set([o])), F(() => {
-                s.delete(o), !s.size && l.delete(i)
+            (s = r.get(i)) ? s.add(o): r.set(i, s = new Set([o])), F(() => {
+                s.delete(o), !s.size && r.delete(i)
             })
         }
-        return n(i, r.value)
+        return n(i, l.value)
     }
 }
 
 function Ie(e) {
     return j(e, !1)
 }
 
@@ -214,28 +214,28 @@
         return e()
     } finally {
         $ = n
     }
 }
 
 function me(e, n, t) {
-    const l = Array.isArray(e);
-    let r, i = t && t.defer;
+    const r = Array.isArray(e);
+    let l, i = t && t.defer;
     return o => {
         let s;
-        if (l) {
+        if (r) {
             s = Array(e.length);
             for (let c = 0; c < e.length; c++) s[c] = e[c]()
         } else s = e();
         if (i) {
             i = !1;
             return
         }
-        const f = I(() => n(s, r, o));
-        return r = s, f
+        const f = I(() => n(s, l, o));
+        return l = s, f
     }
 }
 
 function ke(e) {
     J(() => I(e))
 }
 
@@ -254,47 +254,47 @@
         const e = this.observers ? this.observers.length : 0;
         $.sources ? ($.sources.push(this), $.sourceSlots.push(e)) : ($.sources = [this], $.sourceSlots = [e]), this.observers ? (this.observers.push($), this.observerSlots.push($.sources.length - 1)) : (this.observers = [$], this.observerSlots = [$.sources.length - 1])
     }
     return this.value
 }
 
 function Ne(e, n, t) {
-    let l = e.value;
-    return (!e.comparator || !e.comparator(l, n)) && (e.value = n, e.observers && e.observers.length && j(() => {
-        for (let r = 0; r < e.observers.length; r += 1) {
-            const i = e.observers[r],
+    let r = e.value;
+    return (!e.comparator || !e.comparator(r, n)) && (e.value = n, e.observers && e.observers.length && j(() => {
+        for (let l = 0; l < e.observers.length; l += 1) {
+            const i = e.observers[l],
                 o = se && se.running;
             o && se.disposed.has(i), (o ? !i.tState : !i.state) && (i.pure ? A.push(i) : V.push(i), i.observers && Te(i)), o || (i.state = O)
         }
         if (A.length > 1e6) throw A = [], new Error
     }, !1)), n
 }
 
 function R(e) {
     if (!e.fn) return;
-    re(e);
+    le(e);
     const n = C,
         t = $,
-        l = le;
-    $ = C = e, Ve(e, e.value, l), $ = t, C = n
+        r = re;
+    $ = C = e, Ve(e, e.value, r), $ = t, C = n
 }
 
 function Ve(e, n, t) {
-    let l;
+    let r;
     try {
-        l = e.fn(n)
-    } catch (r) {
-        return e.pure && (e.state = O, e.owned && e.owned.forEach(re), e.owned = null), e.updatedAt = t + 1, Le(r)
-    }(!e.updatedAt || e.updatedAt <= t) && (e.updatedAt != null && "observers" in e ? Ne(e, l) : e.value = l, e.updatedAt = t)
+        r = e.fn(n)
+    } catch (l) {
+        return e.pure && (e.state = O, e.owned && e.owned.forEach(le), e.owned = null), e.updatedAt = t + 1, Le(l)
+    }(!e.updatedAt || e.updatedAt <= t) && (e.updatedAt != null && "observers" in e ? Ne(e, r) : e.value = r, e.updatedAt = t)
 }
 
-function W(e, n, t, l = O, r) {
+function W(e, n, t, r = O, l) {
     const i = {
         fn: e,
-        state: l,
+        state: r,
         updatedAt: null,
         owned: null,
         sources: null,
         sourceSlots: null,
         cleanups: null,
         value: n,
         owner: C,
@@ -306,32 +306,32 @@
 
 function ee(e) {
     if (e.state === 0) return;
     if (e.state === Y) return te(e);
     if (e.suspense && I(e.suspense.inFallback)) return e.suspense.effects.push(e);
     const n = [e];
     for (;
-        (e = e.owner) && (!e.updatedAt || e.updatedAt < le);) e.state && n.push(e);
+        (e = e.owner) && (!e.updatedAt || e.updatedAt < re);) e.state && n.push(e);
     for (let t = n.length - 1; t >= 0; t--)
         if (e = n[t], e.state === O) R(e);
         else if (e.state === Y) {
-        const l = A;
-        A = null, j(() => te(e, n[0]), !1), A = l
+        const r = A;
+        A = null, j(() => te(e, n[0]), !1), A = r
     }
 }
 
 function j(e, n) {
     if (A) return e();
     let t = !1;
-    n || (A = []), V ? t = !0 : V = [], le++;
+    n || (A = []), V ? t = !0 : V = [], re++;
     try {
-        const l = e();
-        return je(t), l
-    } catch (l) {
-        t || (V = null), A = null, Le(l)
+        const r = e();
+        return je(t), r
+    } catch (r) {
+        t || (V = null), A = null, Le(r)
     }
 }
 
 function je(e) {
     if (A && (Pe(A), A = null), e) return;
     const n = V;
     V = null, n.length && j(() => Ee(n), !1)
@@ -340,53 +340,53 @@
 function Pe(e) {
     for (let n = 0; n < e.length; n++) ee(e[n])
 }
 
 function Ue(e) {
     let n, t = 0;
     for (n = 0; n < e.length; n++) {
-        const l = e[n];
-        l.user ? e[t++] = l : ee(l)
+        const r = e[n];
+        r.user ? e[t++] = r : ee(r)
     }
     for (n = 0; n < t; n++) ee(e[n])
 }
 
 function te(e, n) {
     e.state = 0;
     for (let t = 0; t < e.sources.length; t += 1) {
-        const l = e.sources[t];
-        if (l.sources) {
-            const r = l.state;
-            r === O ? l !== n && (!l.updatedAt || l.updatedAt < le) && ee(l) : r === Y && te(l, n)
+        const r = e.sources[t];
+        if (r.sources) {
+            const l = r.state;
+            l === O ? r !== n && (!r.updatedAt || r.updatedAt < re) && ee(r) : l === Y && te(r, n)
         }
     }
 }
 
 function Te(e) {
     for (let n = 0; n < e.observers.length; n += 1) {
         const t = e.observers[n];
         t.state || (t.state = Y, t.pure ? A.push(t) : V.push(t), t.observers && Te(t))
     }
 }
 
-function re(e) {
+function le(e) {
     let n;
     if (e.sources)
         for (; e.sources.length;) {
             const t = e.sources.pop(),
-                l = e.sourceSlots.pop(),
-                r = t.observers;
-            if (r && r.length) {
-                const i = r.pop(),
+                r = e.sourceSlots.pop(),
+                l = t.observers;
+            if (l && l.length) {
+                const i = l.pop(),
                     o = t.observerSlots.pop();
-                l < r.length && (i.sourceSlots[o] = l, r[l] = i, t.observerSlots[l] = o)
+                r < l.length && (i.sourceSlots[o] = r, l[r] = i, t.observerSlots[r] = o)
             }
         }
     if (e.owned) {
-        for (n = e.owned.length - 1; n >= 0; n--) re(e.owned[n]);
+        for (n = e.owned.length - 1; n >= 0; n--) le(e.owned[n]);
         e.owned = null
     }
     if (e.cleanups) {
         for (n = e.cleanups.length - 1; n >= 0; n--) e.cleanups[n]();
         e.cleanups = null
     }
     e.state = 0, e.context = null
@@ -404,38 +404,38 @@
 const Be = Symbol("fallback");
 
 function ye(e) {
     for (let n = 0; n < e.length; n++) e[n]()
 }
 
 function Re(e, n, t = {}) {
-    let l = [],
-        r = [],
+    let r = [],
+        l = [],
         i = [],
         o = 0,
         s = n.length > 1 ? [] : null;
     return F(() => ye(i)), () => {
         let f = e() || [],
             c, a;
         return f[Oe], I(() => {
             let u = f.length,
-                h, d, N, T, L, p, y, w, g;
-            if (u === 0) o !== 0 && (ye(i), i = [], l = [], r = [], o = 0, s && (s = [])), t.fallback && (l = [Be], r[0] = Q(v => (i[0] = v, t.fallback())), o = 1);
+                h, d, N, T, L, _, y, v, g;
+            if (u === 0) o !== 0 && (ye(i), i = [], r = [], l = [], o = 0, s && (s = [])), t.fallback && (r = [Be], l[0] = Q(w => (i[0] = w, t.fallback())), o = 1);
             else if (o === 0) {
-                for (r = new Array(u), a = 0; a < u; a++) l[a] = f[a], r[a] = Q(m);
+                for (l = new Array(u), a = 0; a < u; a++) r[a] = f[a], l[a] = Q(m);
                 o = u
             } else {
-                for (N = new Array(u), T = new Array(u), s && (L = new Array(u)), p = 0, y = Math.min(o, u); p < y && l[p] === f[p]; p++);
-                for (y = o - 1, w = u - 1; y >= p && w >= p && l[y] === f[w]; y--, w--) N[w] = r[y], T[w] = i[y], s && (L[w] = s[y]);
-                for (h = new Map, d = new Array(w + 1), a = w; a >= p; a--) g = f[a], c = h.get(g), d[a] = c === void 0 ? -1 : c, h.set(g, a);
-                for (c = p; c <= y; c++) g = l[c], a = h.get(g), a !== void 0 && a !== -1 ? (N[a] = r[c], T[a] = i[c], s && (L[a] = s[c]), a = d[a], h.set(g, a)) : i[c]();
-                for (a = p; a < u; a++) a in N ? (r[a] = N[a], i[a] = T[a], s && (s[a] = L[a], s[a](a))) : r[a] = Q(m);
-                r = r.slice(0, o = u), l = f.slice(0)
+                for (N = new Array(u), T = new Array(u), s && (L = new Array(u)), _ = 0, y = Math.min(o, u); _ < y && r[_] === f[_]; _++);
+                for (y = o - 1, v = u - 1; y >= _ && v >= _ && r[y] === f[v]; y--, v--) N[v] = l[y], T[v] = i[y], s && (L[v] = s[y]);
+                for (h = new Map, d = new Array(v + 1), a = v; a >= _; a--) g = f[a], c = h.get(g), d[a] = c === void 0 ? -1 : c, h.set(g, a);
+                for (c = _; c <= y; c++) g = r[c], a = h.get(g), a !== void 0 && a !== -1 ? (N[a] = l[c], T[a] = i[c], s && (L[a] = s[c]), a = d[a], h.set(g, a)) : i[c]();
+                for (a = _; a < u; a++) a in N ? (l[a] = N[a], i[a] = T[a], s && (s[a] = L[a], s[a](a))) : l[a] = Q(m);
+                l = l.slice(0, o = u), r = f.slice(0)
             }
-            return r
+            return l
         });
 
         function m(u) {
             if (i[a] = u, s) {
                 const [h, d] = M(a);
                 return s[a] = d, n(f[a], h)
             }
@@ -445,257 +445,257 @@
 }
 
 function k(e, n) {
     return I(() => e(n || {}))
 }
 const Ge = e => `Stale read from <${e}>.`;
 
-function ve(e) {
+function we(e) {
     const n = "fallback" in e && {
         fallback: () => e.fallback
     };
     return Z(Re(() => e.each, e.children, n || void 0))
 }
 
 function qe(e) {
     const n = e.keyed,
         t = Z(() => e.when, void 0, {
-            equals: (l, r) => n ? l === r : !l == !r
+            equals: (r, l) => n ? r === l : !r == !l
         });
     return Z(() => {
-        const l = t();
-        if (l) {
-            const r = e.children;
-            return typeof r == "function" && r.length > 0 ? I(() => r(n ? l : () => {
+        const r = t();
+        if (r) {
+            const l = e.children;
+            return typeof l == "function" && l.length > 0 ? I(() => l(n ? r : () => {
                 if (!I(t)) throw Ge("Show");
                 return e.when
-            })) : r
+            })) : l
         }
         return e.fallback
     }, void 0, void 0)
 }
 
 function He(e, n, t) {
-    let l = t.length,
-        r = n.length,
-        i = l,
+    let r = t.length,
+        l = n.length,
+        i = r,
         o = 0,
         s = 0,
-        f = n[r - 1].nextSibling,
+        f = n[l - 1].nextSibling,
         c = null;
-    for (; o < r || s < i;) {
+    for (; o < l || s < i;) {
         if (n[o] === t[s]) {
             o++, s++;
             continue
         }
-        for (; n[r - 1] === t[i - 1];) r--, i--;
-        if (r === o) {
-            const a = i < l ? s ? t[s - 1].nextSibling : t[i - s] : f;
+        for (; n[l - 1] === t[i - 1];) l--, i--;
+        if (l === o) {
+            const a = i < r ? s ? t[s - 1].nextSibling : t[i - s] : f;
             for (; s < i;) e.insertBefore(t[s++], a)
         } else if (i === s)
-            for (; o < r;)(!c || !c.has(n[o])) && n[o].remove(), o++;
-        else if (n[o] === t[i - 1] && t[s] === n[r - 1]) {
-            const a = n[--r].nextSibling;
-            e.insertBefore(t[s++], n[o++].nextSibling), e.insertBefore(t[--i], a), n[r] = t[i]
+            for (; o < l;)(!c || !c.has(n[o])) && n[o].remove(), o++;
+        else if (n[o] === t[i - 1] && t[s] === n[l - 1]) {
+            const a = n[--l].nextSibling;
+            e.insertBefore(t[s++], n[o++].nextSibling), e.insertBefore(t[--i], a), n[l] = t[i]
         } else {
             if (!c) {
                 c = new Map;
                 let m = s;
                 for (; m < i;) c.set(t[m], m++)
             }
             const a = c.get(n[o]);
             if (a != null)
                 if (s < a && a < i) {
                     let m = o,
                         u = 1,
                         h;
-                    for (; ++m < r && m < i && !((h = c.get(n[m])) == null || h !== a + u);) u++;
+                    for (; ++m < l && m < i && !((h = c.get(n[m])) == null || h !== a + u);) u++;
                     if (u > a - s) {
                         const d = n[o];
                         for (; s < a;) e.insertBefore(t[s++], d)
                     } else e.replaceChild(t[s++], n[o++])
                 } else o++;
             else n[o++].remove()
         }
     }
 }
-const we = "_$DX_DELEGATE";
+const ve = "_$DX_DELEGATE";
 
-function Ke(e, n, t, l = {}) {
-    let r;
+function Ke(e, n, t, r = {}) {
+    let l;
     return Q(i => {
-        r = i, n === document ? e() : b(n, e(), n.firstChild ? null : void 0, t)
-    }, l.owner), () => {
-        r(), n.textContent = ""
+        l = i, n === document ? e() : b(n, e(), n.firstChild ? null : void 0, t)
+    }, r.owner), () => {
+        l(), n.textContent = ""
     }
 }
 
 function U(e, n, t) {
-    let l;
-    const r = () => {
+    let r;
+    const l = () => {
             const o = document.createElement("template");
             return o.innerHTML = e, t ? o.content.firstChild.firstChild : o.content.firstChild
         },
-        i = n ? () => (l || (l = r())).cloneNode(!0) : () => I(() => document.importNode(l || (l = r()), !0));
+        i = n ? () => (r || (r = l())).cloneNode(!0) : () => I(() => document.importNode(r || (r = l()), !0));
     return i.cloneNode = i, i
 }
 
 function ze(e, n = window.document) {
-    const t = n[we] || (n[we] = new Set);
-    for (let l = 0, r = e.length; l < r; l++) {
-        const i = e[l];
+    const t = n[ve] || (n[ve] = new Set);
+    for (let r = 0, l = e.length; r < l; r++) {
+        const i = e[r];
         t.has(i) || (t.add(i), n.addEventListener(i, Je))
     }
 }
 
 function q(e, n) {
     n == null ? e.removeAttribute("class") : e.className = n
 }
 
-function b(e, n, t, l) {
-    if (t !== void 0 && !l && (l = []), typeof n != "function") return ne(e, n, l, t);
-    H(r => ne(e, n(), r, t), l)
+function b(e, n, t, r) {
+    if (t !== void 0 && !r && (r = []), typeof n != "function") return ne(e, n, r, t);
+    H(l => ne(e, n(), l, t), r)
 }
 
 function Je(e) {
     const n = `$$${e.type}`;
     let t = e.composedPath && e.composedPath()[0] || e.target;
     for (e.target !== t && Object.defineProperty(e, "target", {
             configurable: !0,
             value: t
         }), Object.defineProperty(e, "currentTarget", {
             configurable: !0,
             get() {
                 return t || document
             }
         }); t;) {
-        const l = t[n];
-        if (l && !t.disabled) {
-            const r = t[`${n}Data`];
-            if (r !== void 0 ? l.call(t, r, e) : l.call(t, e), e.cancelBubble) return
+        const r = t[n];
+        if (r && !t.disabled) {
+            const l = t[`${n}Data`];
+            if (l !== void 0 ? r.call(t, l, e) : r.call(t, e), e.cancelBubble) return
         }
         t = t._$host || t.parentNode || t.host
     }
 }
 
-function ne(e, n, t, l, r) {
+function ne(e, n, t, r, l) {
     for (; typeof t == "function";) t = t();
     if (n === t) return t;
     const i = typeof n,
-        o = l !== void 0;
+        o = r !== void 0;
     if (e = o && t[0] && t[0].parentNode || e, i === "string" || i === "number")
         if (i === "number" && (n = n.toString()), o) {
             let s = t[0];
-            s && s.nodeType === 3 ? s.data = n : s = document.createTextNode(n), t = G(e, t, l, s)
+            s && s.nodeType === 3 ? s.data = n : s = document.createTextNode(n), t = G(e, t, r, s)
         } else t !== "" && typeof t == "string" ? t = e.firstChild.data = n : t = e.textContent = n;
-    else if (n == null || i === "boolean") t = G(e, t, l);
+    else if (n == null || i === "boolean") t = G(e, t, r);
     else {
         if (i === "function") return H(() => {
             let s = n();
             for (; typeof s == "function";) s = s();
-            t = ne(e, s, t, l)
+            t = ne(e, s, t, r)
         }), () => t;
         if (Array.isArray(n)) {
             const s = [],
                 f = t && Array.isArray(t);
-            if (ae(s, n, t, r)) return H(() => t = ne(e, s, t, l, !0)), () => t;
+            if (ae(s, n, t, l)) return H(() => t = ne(e, s, t, r, !0)), () => t;
             if (s.length === 0) {
-                if (t = G(e, t, l), o) return t
-            } else f ? t.length === 0 ? be(e, s, l) : He(e, t, s) : (t && G(e), be(e, s));
+                if (t = G(e, t, r), o) return t
+            } else f ? t.length === 0 ? be(e, s, r) : He(e, t, s) : (t && G(e), be(e, s));
             t = s
         } else if (n instanceof Node) {
             if (Array.isArray(t)) {
-                if (o) return t = G(e, t, l, n);
+                if (o) return t = G(e, t, r, n);
                 G(e, t, null, n)
             } else t == null || t === "" || !e.firstChild ? e.appendChild(n) : e.replaceChild(n, e.firstChild);
             t = n
         } else console.warn("Unrecognized value. Skipped inserting", n)
     }
     return t
 }
 
-function ae(e, n, t, l) {
-    let r = !1;
+function ae(e, n, t, r) {
+    let l = !1;
     for (let i = 0, o = n.length; i < o; i++) {
         let s = n[i],
             f = t && t[i];
         if (s instanceof Node) e.push(s);
         else if (!(s == null || s === !0 || s === !1))
-            if (Array.isArray(s)) r = ae(e, s, f) || r;
+            if (Array.isArray(s)) l = ae(e, s, f) || l;
             else if (typeof s == "function")
-            if (l) {
+            if (r) {
                 for (; typeof s == "function";) s = s();
-                r = ae(e, Array.isArray(s) ? s : [s], Array.isArray(f) ? f : [f]) || r
-            } else e.push(s), r = !0;
+                l = ae(e, Array.isArray(s) ? s : [s], Array.isArray(f) ? f : [f]) || l
+            } else e.push(s), l = !0;
         else {
             const c = String(s);
             f && f.nodeType === 3 ? (f.data = c, e.push(f)) : e.push(document.createTextNode(c))
         }
     }
-    return r
+    return l
 }
 
 function be(e, n, t = null) {
-    for (let l = 0, r = n.length; l < r; l++) e.insertBefore(n[l], t)
+    for (let r = 0, l = n.length; r < l; r++) e.insertBefore(n[r], t)
 }
 
-function G(e, n, t, l) {
+function G(e, n, t, r) {
     if (t === void 0) return e.textContent = "";
-    const r = l || document.createTextNode("");
+    const l = r || document.createTextNode("");
     if (n.length) {
         let i = !1;
         for (let o = n.length - 1; o >= 0; o--) {
             const s = n[o];
-            if (r !== s) {
+            if (l !== s) {
                 const f = s.parentNode === e;
-                !i && !o ? f ? e.replaceChild(r, s) : e.insertBefore(r, t) : f && s.remove()
+                !i && !o ? f ? e.replaceChild(l, s) : e.insertBefore(l, t) : f && s.remove()
             } else i = !0
         }
-    } else e.insertBefore(r, t);
-    return [r]
+    } else e.insertBefore(l, t);
+    return [l]
 }
 var Fe = ["Shift", "Meta", "Alt", "Control"],
     We = typeof navigator == "object" && /Mac|iPod|iPhone|iPad/.test(navigator.platform) ? "Meta" : "Control";
 
 function oe(e, n) {
     return typeof e.getModifierState == "function" && e.getModifierState(n)
 }
 
 function Qe(e) {
     return e.trim().split(" ").map(function(n) {
         var t = n.split(/\b\+/),
-            l = t.pop();
-        return [t = t.map(function(r) {
-            return r === "$mod" ? We : r
-        }), l]
+            r = t.pop();
+        return [t = t.map(function(l) {
+            return l === "$mod" ? We : l
+        }), r]
     })
 }
 
 function Xe(e, n) {
     var t;
     n === void 0 && (n = {});
-    var l = (t = n.timeout) != null ? t : 1e3,
-        r = Object.keys(e).map(function(s) {
+    var r = (t = n.timeout) != null ? t : 1e3,
+        l = Object.keys(e).map(function(s) {
             return [Qe(s), e[s]]
         }),
         i = new Map,
         o = null;
     return function(s) {
-        s instanceof KeyboardEvent && (r.forEach(function(f) {
+        s instanceof KeyboardEvent && (l.forEach(function(f) {
             var c = f[0],
                 a = f[1],
                 m = i.get(c) || c;
             (function(u, h) {
                 return !(h[1].toUpperCase() !== u.key.toUpperCase() && h[1] !== u.code || h[0].find(function(d) {
                     return !oe(u, d)
                 }) || Fe.find(function(d) {
                     return !h[0].includes(d) && h[1] !== d && oe(u, d)
                 }))
             })(s, m[0]) ? m.length > 1 ? i.set(c, m.slice(1)) : (i.delete(c), a(s)): oe(s, s.key) || i.delete(c)
-        }), o && clearTimeout(o), o = setTimeout(i.clear.bind(i), l))
+        }), o && clearTimeout(o), o = setTimeout(i.clear.bind(i), r))
     }
 }
 const Ye = e => `http://127.0.0.1:8000${e}`;
 
 function Ze() {
     const e = async (n, t) => (await fetch(Ye(n), {
         method: "POST",
@@ -718,135 +718,135 @@
 
 function et(e, n, t) {
     return M(n(), t)
 }
 var tt = et;
 
 function xe(e, n, t) {
-    const [l, r] = M(), i = t != null && t.api ? Array.isArray(t.api) ? t.api : [t.api] : [globalThis.localStorage].filter(Boolean), o = t != null && t.prefix ? `${t.prefix}.` : "", s = () => i.reduce((m, u) => {
+    const [r, l] = M(), i = t != null && t.api ? Array.isArray(t.api) ? t.api : [t.api] : [globalThis.localStorage].filter(Boolean), o = t != null && t.prefix ? `${t.prefix}.` : "", s = () => i.reduce((m, u) => {
         if (m !== null || !u) return m;
         let h = null;
         try {
             h = u.getItem(`${o}${e}`)
         } catch (d) {
-            if (r(d instanceof Error ? d : new Error(`Error reading ${o}${e} from ${u.name}`)), t != null && t.throw) throw d
+            if (l(d instanceof Error ? d : new Error(`Error reading ${o}${e} from ${u.name}`)), t != null && t.throw) throw d
         }
         return h !== null && (t != null && t.deserializer) ? t.deserializer(h + "", e, t.options) : h
     }, null), [f, c] = tt(n, () => s() ?? n, t);
     J(() => {
         const m = f(),
             u = t != null && t.serializer ? t.serializer(m, e, t.options) : m + "",
             h = `${o}${e}`;
         try {
             m === null ? i.forEach(d => d.getItem(h) !== null && d.removeItem(h)) : i.forEach(d => d.getItem(h) !== u && d.setItem(h, u, t == null ? void 0 : t.options))
         } catch (d) {
-            if (r(d instanceof Error ? d : new Error(`Error ${m===null?"removing":"writing"} value`)), t != null && t.throw) throw d
+            if (l(d instanceof Error ? d : new Error(`Error ${m===null?"removing":"writing"} value`)), t != null && t.throw) throw d
         }
     });
     const a = () => {
         const m = s();
         c(m)
     };
     return (t == null ? void 0 : t.sync) !== !1 && ke(() => {
         const m = u => {
             let h = !1;
             try {
                 i.forEach(d => {
                     d !== u.storageArea && u.key && u.newValue !== d.getItem(u.key) && (u.newValue ? d.setItem(u.key, u.newValue) : d.removeItem(u.key), h = !0)
                 })
             } catch (d) {
-                if (r(d instanceof Error ? d : new Error("Error synching api after event")), t != null && t.throw) throw d
+                if (l(d instanceof Error ? d : new Error("Error synching api after event")), t != null && t.throw) throw d
             }
             h && a()
         };
         "addEventListener" in globalThis ? (globalThis.addEventListener("storage", m), F(() => globalThis.removeEventListener("storage", m))) : (i.forEach(u => {
             var h;
             return (h = u.addEventListener) == null ? void 0 : h.call(u, "storage", m)
         }), F(() => i.forEach(u => {
             var h;
             return (h = u.removeEventListener) == null ? void 0 : h.call(u, "storage", m)
         })))
     }), [Object.assign(f, {
-        error: l
+        error: r
     }), c, a]
 }
 var nt = e => (typeof e.clear == "function" || (e.clear = () => {
         let n;
         for (; n = e.key(0);) e.removeItem(n)
     }), e),
     $e = e => {
         if (!e) return "";
         let n = "";
         for (const t in e) {
             if (!e.hasOwnProperty(t)) continue;
-            const l = e[t];
-            n += l instanceof Date ? `; ${t}=${l.toUTCString()}` : typeof l == "boolean" ? `; ${t}` : `; ${t}=${l}`
+            const r = e[t];
+            n += r instanceof Date ? `; ${t}=${r.toUTCString()}` : typeof r == "boolean" ? `; ${t}` : `; ${t}=${r}`
         }
         return n
     },
     P = nt({
         _cookies: [globalThis.document, "cookie"],
         getItem: e => {
             var n;
             return ((n = P._cookies[0][P._cookies[1]].match("(^|;)\\s*" + e + "\\s*=\\s*([^;]+)")) == null ? void 0 : n.pop()) ?? null
         },
         setItem: (e, n, t) => {
-            const l = P.getItem(e);
+            const r = P.getItem(e);
             P._cookies[0][P._cookies[1]] = `${e}=${n}${$e(t)}`;
-            const r = Object.assign(new Event("storage"), {
+            const l = Object.assign(new Event("storage"), {
                 key: e,
-                oldValue: l,
+                oldValue: r,
                 newValue: n,
                 url: globalThis.document.URL,
                 storageArea: P
             });
-            window.dispatchEvent(r)
+            window.dispatchEvent(l)
         },
         removeItem: e => {
             P._cookies[0][P._cookies[1]] = `${e}=deleted${$e({expires:new Date(0)})}`
         },
         key: e => {
             let n = null,
                 t = 0;
-            return P._cookies[0][P._cookies[1]].replace(/(?:^|;)\s*(.+?)\s*=\s*[^;]+/g, (l, r) => (!n && r && t++ === e && (n = r), "")), n
+            return P._cookies[0][P._cookies[1]].replace(/(?:^|;)\s*(.+?)\s*=\s*[^;]+/g, (r, l) => (!n && l && t++ === e && (n = l), "")), n
         },
         get length() {
             let e = 0;
             return P._cookies[0][P._cookies[1]].replace(/(?:^|;)\s*.+?\s*=\s*[^;]+/g, n => (e += n ? 1 : 0, "")), e
         }
     });
 
-function lt(e, n) {
+function rt(e, n) {
     if (!n) return;
     const t = e.indexOf(n);
     return e.at(t - 1)
 }
 
-function rt(e, n) {
+function lt(e, n) {
     if (!n) return e[0];
     const t = e.indexOf(n);
     return e.at(t + 1) || e[0]
 }
 
 function it(e) {
     const [n, {
         refetch: t
     }] = ge(e.get_setlists);
 
-    function l(g, v) {
-        return m() && g && v && g !== v ? confirm("Change current setlist?") : !0
+    function r(g, w) {
+        return m() && g && w && g !== w ? confirm("Change current setlist?") : !0
     }
-    const [r, i] = xe("setlistName", null, {
-        equals: (g, v) => !l(g, v)
+    const [l, i] = xe("setlistName", null, {
+        equals: (g, w) => !r(g, w)
     }), [o, {
         refetch: s
-    }] = ge(r, e.get_setlist);
+    }] = ge(l, e.get_setlist);
     J(me(o, g => {
-        const v = f();
-        g && g.songs && (g.songs.find(x => x.name == (v == null ? void 0 : v.name)) || c(g.songs[0]))
+        const w = f();
+        g && g.songs && (g.songs.find(x => x.name == (w == null ? void 0 : w.name)) || c(g.songs[0]))
     }));
     const [f, c] = xe("song", null, {
         serializer: g => {
             try {
                 return JSON.stringify(g)
             } catch {
                 return null
@@ -871,180 +871,180 @@
     }
     const [m, u] = M(!1);
     async function h() {
         const g = f();
         g && a(await e.toggle_playing(g.tempo))
     }
     const [d, N] = M(!0), T = async () => a(await e.toggle_guide_enabled()), L = async () => a(await e.reset());
-    let p;
+    let _;
     J(() => {
-        const g = r();
-        p == null || p.close(), p = new WebSocket(`ws://127.0.0.1:8000/watch?current_setlist=${g}`), p.addEventListener("message", v => {
-            v.data == "current_setlist" ? s() : v.data == "setlists" && t()
+        const g = l();
+        _ == null || _.close(), _ = new WebSocket(`ws://127.0.0.1:8000/watch?current_setlist=${g}`), _.addEventListener("message", w => {
+            w.data == "current_setlist" ? s() : w.data == "setlists" && t()
         }, !1)
     });
 
     function y() {
-        var v;
-        const g = (v = o()) == null ? void 0 : v.songs;
+        var w;
+        const g = (w = o()) == null ? void 0 : w.songs;
         if (g) {
-            const E = lt(g, f());
+            const E = rt(g, f());
             E && c(E)
         }
     }
 
-    function w() {
-        var v;
-        const g = (v = o()) == null ? void 0 : v.songs;
-        g && c(rt(g, f()))
+    function v() {
+        var w;
+        const g = (w = o()) == null ? void 0 : w.songs;
+        g && c(lt(g, f()))
     }
     return {
         setlists: n,
-        setlistName: r,
+        setlistName: l,
         setSetlistName: i,
         setlist: o,
         song: f,
         setSong: c,
         togglePlaying: h,
         playing: m,
         toggleGuide: T,
         guideEnabled: d,
         resetPlayback: L,
         previousSong: y,
-        nextSong: w
+        nextSong: v
     }
 }
-const st = U('<div class="grid h-full place-content-center text-gray-500"></div>', 2),
-    ot = U('<div class="h-15 flex w-40 basis-1/4 flex-col place-items-center items-center rounded-lg bg-gray-100 p-3 text-center text-sm"><span class="text-2xl font-semibold"></span><span class=" text-xs font-semibold uppercase"></span></div>', 6),
-    at = U("<div><span><span></span></span><span></span></div>", 8),
-    ct = U('<div class="App grid h-screen" style="grid-template-columns: 1fr 2fr 4fr;"><ul class="overflow-y-scroll px-5"></ul><div class="overflow-y-scroll ring-1 ring-black/5"></div><div class="flex flex-col overflow-hidden"></div></div>', 8),
-    ut = U("<li></li>", 2),
-    ft = U('<div><div><div></div><div class="text-sm"></div></div><div><div class="px-3"></div><div class="px-3"></div><div class="px-3"></div></div></div>', 16),
-    dt = U('<div class="m-20 flex flex-1 flex-col"><div class="text-8xl font-bold"></div><div class="my-2 text-6xl"></div><div class="my-6 flex flex-wrap gap-2"></div></div>', 8),
-    gt = U('<div class="mx-20 mb-10 mt-2 flex flex-col"><hr class="w-full p-2"><div class="flex flex-wrap gap-2"></div></div>', 5);
+const st = U('<div class="grid h-full place-content-center text-gray-500">'),
+    ot = U('<div class="h-15 flex w-40 basis-1/4 flex-col place-items-center items-center rounded-lg bg-gray-100 p-3 text-center text-sm"><span class="text-2xl font-semibold"></span><span class=" text-xs font-semibold uppercase">'),
+    at = U("<div><span><span></span></span><span>"),
+    ct = U('<div class="App grid h-screen" style="grid-template-columns:1fr 2fr 4fr;"><ul class="overflow-y-scroll px-5"></ul><div class="overflow-y-scroll ring-1 ring-black/5"></div><div class="flex flex-col overflow-hidden">'),
+    ut = U("<li>"),
+    ft = U('<div><div><div></div><div class="text-sm"></div></div><div><div class="px-3"></div><div class="px-3"></div><div class="px-3">'),
+    dt = U('<div class="m-20 flex flex-1 flex-col"><div class="text-8xl font-bold"></div><div class="my-2 text-6xl"></div><div class="my-6 flex flex-wrap gap-2">'),
+    gt = U('<div class="mx-20 mb-10 mt-2 flex flex-col"><hr class="w-full p-2"><div class="flex flex-wrap gap-2">');
 
-function pe(e) {
+function _e(e) {
     return (() => {
-        const n = st.cloneNode(!0);
+        const n = st();
         return b(n, () => e.text), n
     })()
 }
 
 function K(e) {
     return (() => {
-        const n = ot.cloneNode(!0),
+        const n = ot(),
             t = n.firstChild,
-            l = t.nextSibling;
-        return b(t, () => e.param), b(l, () => e.name), n
+            r = t.nextSibling;
+        return b(t, () => e.param), b(r, () => e.name), n
     })()
 }
 
-function _e(e, n) {
+function Se(e, n) {
     const t = Xe(n);
     ke(() => window.addEventListener(e, t)), F(() => window.removeEventListener(e, t))
 }
 
 function z(e) {
     const [n, t] = M(!1);
-    return _e("keydown", Object.fromEntries(e.keys.map(l => [l, r => {
-        e.action(r), t(!0)
-    }]))), _e("keyup", Object.fromEntries(e.keys.map(l => [l, () => t(!1)]))), (() => {
-        const l = at.cloneNode(!0),
-            r = l.firstChild,
-            i = r.firstChild,
-            o = r.nextSibling;
+    return Se("keydown", Object.fromEntries(e.keys.map(r => [r, l => {
+        e.action(l), t(!0)
+    }]))), Se("keyup", Object.fromEntries(e.keys.map(r => [r, () => t(!1)]))), (() => {
+        const r = at(),
+            l = r.firstChild,
+            i = l.firstChild,
+            o = l.nextSibling;
         return b(i, () => e.prettyValue), b(o, () => e.name), H(s => {
             const f = `w-max space-x-2 rounded-lg p-2 font-mono text-sm ${n()?"bg-gray-300":"bg-gray-100"}`,
                 c = `rounded-lg ${n()?"bg-gray-300":"bg-gray-200"} p-1 text-sm`;
-            return f !== s._v$ && q(l, s._v$ = f), c !== s._v$2 && q(r, s._v$2 = c), s
+            return f !== s._v$ && q(r, s._v$ = f), c !== s._v$2 && q(l, s._v$2 = c), s
         }, {
             _v$: void 0,
             _v$2: void 0
-        }), l
+        }), r
     })()
 }
 
 function ht() {
     const {
         setlists: e,
         setlistName: n,
         setSetlistName: t,
-        setlist: l,
-        song: r,
+        setlist: r,
+        song: l,
         setSong: i,
         togglePlaying: o,
         playing: s,
         toggleGuide: f,
         guideEnabled: c,
         resetPlayback: a,
         previousSong: m,
         nextSong: u
     } = it(Ze()), h = he(n), d = he(() => {
         var N;
-        return (N = r()) == null ? void 0 : N.name
+        return (N = l()) == null ? void 0 : N.name
     });
     return (() => {
-        const N = ct.cloneNode(!0),
+        const N = ct(),
             T = N.firstChild,
             L = T.nextSibling,
-            p = L.nextSibling;
-        return b(T, k(ve, {
+            _ = L.nextSibling;
+        return b(T, k(we, {
             get each() {
                 return e()
             },
             children: y => (() => {
-                const w = ut.cloneNode(!0);
-                return w.$$click = () => t(y), b(w, y), H(() => q(w, `-ml-[2px] block break-after-left border-l-2 border-gray-100 p-2 pl-4 first:mt-7 last:mb-7 hover:transition-all ${h(y)?"border-yellow-600 text-yellow-600":"text-gray-500 hover:border-black hover:text-black"}`)), w
+                const v = ut();
+                return v.$$click = () => t(y), b(v, y), H(() => q(v, `-ml-[2px] block break-after-left border-l-2 border-gray-100 p-2 pl-4 first:mt-7 last:mb-7 hover:transition-all ${h(y)?"border-yellow-600 text-yellow-600":"text-gray-500 hover:border-black hover:text-black"}`)), v
             })()
-        })), b(L, k(ve, {
+        })), b(L, k(we, {
             get each() {
                 var y;
-                return (y = l()) == null ? void 0 : y.songs
+                return (y = r()) == null ? void 0 : y.songs
             },
             get fallback() {
-                return k(pe, {
+                return k(_e, {
                     text: "Choose a setlist"
                 })
             },
             children: y => (() => {
-                const w = ft.cloneNode(!0),
-                    g = w.firstChild,
-                    v = g.firstChild,
-                    E = v.nextSibling,
+                const v = ft(),
+                    g = v.firstChild,
+                    w = g.firstChild,
+                    E = w.nextSibling,
                     x = g.nextSibling,
-                    _ = x.firstChild,
-                    S = _.nextSibling,
-                    D = S.nextSibling;
-                return w.$$click = () => i(y), b(v, () => y.name), b(E, () => y.artist), b(_, () => y.tempo.bpm), b(S, () => y.tempo.time_signature), b(D, () => y.tempo.duration), H(B => {
+                    S = x.firstChild,
+                    p = S.nextSibling,
+                    D = p.nextSibling;
+                return v.$$click = () => i(y), b(w, () => y.name), b(E, () => y.artist), b(S, () => y.tempo.bpm), b(p, () => y.tempo.time_signature), b(D, () => y.tempo.duration), H(B => {
                     const ce = `group flex border border-gray-100 first:mt-7 last:mb-7 hover:bg-gray-50 ${d(y.name)?"bg-gray-50":""}`,
                         ue = `flex-grow p-4 pl-8 ${d(y.name)?"text-yellow-700":"text-gray-500 hover:text-black"}`,
                         fe = `invisible grid grid-cols-3 place-items-center divide-x whitespace-nowrap pr-6 text-sm group-hover:visible ${d(y.name)?"divide-yellow-700 text-yellow-700":"divide-gray-500 text-gray-500"}`;
-                    return ce !== B._v$3 && q(w, B._v$3 = ce), ue !== B._v$4 && q(g, B._v$4 = ue), fe !== B._v$5 && q(x, B._v$5 = fe), B
+                    return ce !== B._v$3 && q(v, B._v$3 = ce), ue !== B._v$4 && q(g, B._v$4 = ue), fe !== B._v$5 && q(x, B._v$5 = fe), B
                 }, {
                     _v$3: void 0,
                     _v$4: void 0,
                     _v$5: void 0
-                }), w
+                }), v
             })()
-        })), b(p, k(qe, {
+        })), b(_, k(qe, {
             get when() {
-                return r()
+                return l()
             },
             get fallback() {
-                return k(pe, {
+                return k(_e, {
                     text: "Choose a song"
                 })
             },
             keyed: !0,
             children: y => [(() => {
-                const w = dt.cloneNode(!0),
-                    g = w.firstChild,
-                    v = g.nextSibling,
-                    E = v.nextSibling;
-                return b(g, () => y.name), b(v, () => y.artist), b(E, k(K, {
+                const v = dt(),
+                    g = v.firstChild,
+                    w = g.nextSibling,
+                    E = w.nextSibling;
+                return b(g, () => y.name), b(w, () => y.artist), b(E, k(K, {
                     name: "Tempo",
                     get param() {
                         return `${y.tempo.bpm}`
                     }
                 }), null), b(E, k(K, {
                     name: "Time Signature",
                     get param() {
@@ -1061,47 +1061,47 @@
                         return `${s()?"Playing":"Paused"}`
                     }
                 }), null), b(E, k(K, {
                     name: "Guide",
                     get param() {
                         return `${c()?"Enabled":"Disabled"}`
                     }
-                }), null), w
+                }), null), v
             })(), (() => {
-                const w = gt.cloneNode(!0),
-                    g = w.firstChild,
-                    v = g.nextSibling;
-                return b(v, k(z, {
+                const v = gt(),
+                    g = v.firstChild,
+                    w = g.nextSibling;
+                return b(w, k(z, {
                     name: "Play/Pause",
                     prettyValue: "Space",
                     keys: ["Space"],
                     action: async E => {
                         E.preventDefault(), await o()
                     }
-                }), null), b(v, k(z, {
+                }), null), b(w, k(z, {
                     name: "Reset",
                     prettyValue: "R",
                     keys: ["r", "к"],
                     action: a
-                }), null), b(v, k(z, {
+                }), null), b(w, k(z, {
                     name: "Toggle Guide",
                     prettyValue: "G",
                     keys: ["g", "п"],
                     action: f
-                }), null), b(v, k(z, {
+                }), null), b(w, k(z, {
                     name: "Previous Song",
                     prettyValue: "←",
                     keys: ["ArrowLeft"],
                     action: m
-                }), null), b(v, k(z, {
+                }), null), b(w, k(z, {
                     name: "Next Song",
                     prettyValue: "→",
                     keys: ["ArrowRight"],
                     action: u
-                }), null), w
+                }), null), v
             })()]
         })), N
     })()
 }
 ze(["click"]);
 addEventListener("error", e => alert(e.error));
 Ke(() => k(ht, {}), document.getElementById("root"));
```

### Comparing `playbacker-0.5.0/src/playbacker/dist/assets/index-c1f1d727.css` & `playbacker-0.5.1/src/playbacker/dist/assets/index-c1f1d727.css`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.0/src/playbacker/main.py` & `playbacker-0.5.1/src/playbacker/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,24 +68,24 @@
     config_file = get_config_file_path(config)
     songs_file = get_songs_file_path(config)
     setlists_dir = get_setlists_dir_path(config)
 
     with Progress(
         SpinnerColumn(), TextColumn("[progress.description]{task.description}")
     ) as progress:
-        progress.add_task(description="Formatting...")
-        format_yaml_files(config_file, songs_file, f"{setlists_dir}/*.yaml")
-
-        progress.add_task(description="Validating config schema...")
-        validate_config_schema(config_file)
-
         progress.add_task(description="Checking unknown songs...")
         unknown_songs = get_unknown_songs(
             songs_file=songs_file, setlists_dir=setlists_dir
         )
         if unknown_songs:
-            progress.stop()
             table = Table(show_header=False, show_lines=True)
             for setlist_path, songs in unknown_songs.items():
                 songs_str = ",\n".join(f'"{song}"' for song in songs)
                 table.add_row(str(setlist_path), songs_str)
+            progress.stop()
             progress.print("There are unknown songs in setlists:", table)
+
+        progress.add_task(description="Validating config schema...")
+        validate_config_schema(config_file)
+
+        progress.add_task(description="Formatting...")
+        format_yaml_files(config_file, songs_file, f"{setlists_dir}/*.yaml")
```

### Comparing `playbacker-0.5.0/PKG-INFO` & `playbacker-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: playbacker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Live music performance playback
 License: MIT
 Author: Lev Vereshchagin
 Author-email: mail@vrslev.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: SoundFile (==0.12.1)
 Requires-Dist: inquirer (==3.1.3)
-Requires-Dist: numpy (==1.24.2)
+Requires-Dist: numpy (==1.24.3)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: sounddevice (==0.4.6)
-Requires-Dist: soxr (==0.3.4)
-Requires-Dist: starlite (==1.51.9)
+Requires-Dist: soxr (==0.3.5)
+Requires-Dist: starlite (==1.51.10)
 Requires-Dist: typer[all] (==0.7.0)
 Requires-Dist: uvicorn[standard] (==0.21.1)
 Requires-Dist: uvloop (==0.17.0)
 Requires-Dist: watchfiles (==0.19.0)
```

