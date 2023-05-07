# Comparing `tmp/nazo_rand-0.0.8.tar.gz` & `tmp/nazo_rand-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.8.tar", last modified: Sun May  7 10:03:22 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.9.tar", last modified: Sun May  7 10:29:01 2023, max compression
```

## Comparing `nazo_rand-0.0.8.tar` & `nazo_rand-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/
--rw-rw-rw-   0        0        0    18431 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      130 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1971 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/nazo_rand/
--rw-rw-rw-   0        0        0       26 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/__init__.py
--rw-rw-rw-   0        0        0   274726 2023-05-07 10:03:21.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.cpp
--rw-rw-rw-   0        0        0     1954 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.hpp
--rw-rw-rw-   0        0        0      700 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pxd
--rw-rw-rw-   0        0        0     2624 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pyi
--rw-rw-rw-   0        0        0     2572 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pyx
-drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/nazo_rand.egg-info/
--rw-rw-rw-   0        0        0     1971 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      484 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2172 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:29:01.967026 nazo_rand-0.0.9/
+-rw-rw-rw-   0        0        0    18431 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2025 2023-05-07 10:29:01.967026 nazo_rand-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 10:29:01.967026 nazo_rand-0.0.9/nazo_rand/
+-rw-rw-rw-   0        0        0       26 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/nazo_rand/__init__.py
+-rw-rw-rw-   0        0        0   248898 2023-05-07 10:29:01.000000 nazo_rand-0.0.9/nazo_rand/nazo_rand.cpp
+-rw-rw-rw-   0        0        0     1954 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/nazo_rand/nazo_rand.hpp
+-rw-rw-rw-   0        0        0      700 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/nazo_rand/nazo_rand.pxd
+-rw-rw-rw-   0        0        0     2624 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/nazo_rand/nazo_rand.pyi
+-rw-rw-rw-   0        0        0     2566 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/nazo_rand/nazo_rand.pyx
+drwxrwxrwx   0        0        0        0 2023-05-07 10:29:01.967026 nazo_rand-0.0.9/nazo_rand.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-05-07 10:29:01.000000 nazo_rand-0.0.9/nazo_rand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-05-07 10:29:01.000000 nazo_rand-0.0.9/nazo_rand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 10:29:01.000000 nazo_rand-0.0.9/nazo_rand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 10:29:01.000000 nazo_rand-0.0.9/nazo_rand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      507 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 10:29:01.967026 nazo_rand-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2225 2023-05-07 10:28:21.000000 nazo_rand-0.0.9/setup.py
```

### Comparing `nazo_rand-0.0.8/LICENSE` & `nazo_rand-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.8/PKG-INFO` & `nazo_rand-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nazo_rand
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nazo_rand
```

### Comparing `nazo_rand-0.0.8/README.md` & `nazo_rand-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.8/nazo_rand/nazo_rand.cpp` & `nazo_rand-0.0.9/nazo_rand/nazo_rand.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -987,50 +987,14 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "nazo_rand\\nazo_rand.pyx",
 };
-/* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
-struct __Pyx_StructField_;
-#define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
-typedef struct {
-  const char* name;
-  struct __Pyx_StructField_* fields;
-  size_t size;
-  size_t arraysize[8];
-  int ndim;
-  char typegroup;
-  char is_unsigned;
-  int flags;
-} __Pyx_TypeInfo;
-typedef struct __Pyx_StructField_ {
-  __Pyx_TypeInfo* type;
-  const char* name;
-  size_t offset;
-} __Pyx_StructField;
-typedef struct {
-  __Pyx_StructField* field;
-  size_t parent_offset;
-} __Pyx_BufFmt_StackElem;
-typedef struct {
-  __Pyx_StructField root;
-  __Pyx_BufFmt_StackElem* head;
-  size_t fmt_offset;
-  size_t new_count, enc_count;
-  size_t struct_alignment;
-  int is_complex;
-  char enc_type;
-  char new_packmode;
-  char enc_packmode;
-  char is_valid_array;
-} __Pyx_BufFmt_Context;
-
 
 /*--- Type declarations ---*/
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange;
 
 /* "nazo_rand/nazo_rand.pxd":14
  * # def int randbelow(int a)
  * # def int randint(int a,int b)
@@ -1114,37 +1078,24 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* IsLittleEndian.proto */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
-
-/* BufferFormatCheck.proto */
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type);
-
-/* BufferGetAndValidate.proto */
-#define __Pyx_GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack)\
-    ((obj == Py_None || obj == NULL) ?\
-    (__Pyx_ZeroBuffer(buf), 0) :\
-    __Pyx__GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack))
-static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
-    __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
-static void __Pyx_ZeroBuffer(Py_buffer* buf);
-static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
-static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
-static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
+/* SetItemInt.proto */
+#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
+               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
+static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
+                                               int is_list, int wraparound, int boundscheck);
 
-#define __Pyx_BufPtrFull1d(type, buf, i0, s0, o0) (type)(__Pyx_BufPtrFull1d_imp(buf, i0, s0, o0))
-static CYTHON_INLINE void* __Pyx_BufPtrFull1d_imp(void* buf, Py_ssize_t i0, Py_ssize_t s0, Py_ssize_t o0);
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1245,24 +1196,14 @@
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* SetItemInt.proto */
-#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
-               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
-                                               int is_list, int wraparound, int boundscheck);
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1370,37 +1311,14 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* BufferStructDeclare.proto */
-typedef struct {
-  Py_ssize_t shape, strides, suboffsets;
-} __Pyx_Buf_DimInfo;
-typedef struct {
-  size_t refcount;
-  Py_buffer pybuffer;
-} __Pyx_Buffer;
-typedef struct {
-  __Pyx_Buffer *rcbuffer;
-  char *data;
-  __Pyx_Buf_DimInfo diminfo[8];
-} __Pyx_LocalBuf_ND;
-
-#if PY_MAJOR_VERSION < 3
-    static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags);
-    static void __Pyx_ReleaseBuffer(Py_buffer *view);
-#else
-    #define __Pyx_GetBuffer PyObject_GetBuffer
-    #define __Pyx_ReleaseBuffer PyBuffer_Release
-#endif
-
-
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
@@ -1454,15 +1372,14 @@
 static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_sample(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
-static __Pyx_TypeInfo __Pyx_TypeInfo_object = { "Python object", NULL, sizeof(PyObject *), { 0 }, 0, 'O', 0, 0 };
 #define __Pyx_MODULE_NAME "nazo_rand.nazo_rand"
 extern int __pyx_module_is_main_nazo_rand__nazo_rand;
 int __pyx_module_is_main_nazo_rand__nazo_rand = 0;
 
 /* Implementation of 'nazo_rand.nazo_rand' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
@@ -1638,15 +1555,15 @@
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
 
   /* "nazo_rand/nazo_rand.pyx":22
  * 
  * cpdef int random_integer_noargs():
  *     return uniform_int_variate_noargs()             # <<<<<<<<<<<<<<
  * 
- * cpdef void shuffle(list[object] array):
+ * cpdef void shuffle(list array):
  */
   __pyx_r = Storm::uniform_int_variate_noargs();
   goto __pyx_L0;
 
   /* "nazo_rand/nazo_rand.pyx":21
  *     return uniform_int_variate(a, b)
  * 
@@ -1700,55 +1617,46 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef object temp
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
 static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *__pyx_v_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_i;
   int __pyx_v_j;
   PyObject *__pyx_v_temp = 0;
   int __pyx_v_length;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
-  __Pyx_Buffer __pyx_pybuffer_array;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject **__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
-  __pyx_pybuffer_array.pybuffer.buf = NULL;
-  __pyx_pybuffer_array.refcount = 0;
-  __pyx_pybuffernd_array.data = NULL;
-  __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_INDIRECT| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[0].suboffsets = __pyx_pybuffernd_array.rcbuffer->pybuffer.suboffsets[0];
 
   /* "nazo_rand/nazo_rand.pyx":27
  *     cdef int i, j
  *     cdef object temp
  *     cdef int length = len(array)             # <<<<<<<<<<<<<<
  *     for i in range(length - 1, 0, -1):
  *         j = cy_uniform_int_variate(0, i)
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (unlikely(__pyx_v_array == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 27, __pyx_L1_error)
+  }
+  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
   /* "nazo_rand/nazo_rand.pyx":28
  *     cdef object temp
  *     cdef int length = len(array)
  *     for i in range(length - 1, 0, -1):             # <<<<<<<<<<<<<<
  *         j = cy_uniform_int_variate(0, i)
@@ -1769,78 +1677,71 @@
     /* "nazo_rand/nazo_rand.pyx":30
  *     for i in range(length - 1, 0, -1):
  *         j = cy_uniform_int_variate(0, i)
  *         temp = array[i]             # <<<<<<<<<<<<<<
  *         array[i] = array[j]
  *         array[j] = temp
  */
-    __pyx_t_4 = __pyx_v_i;
-    __pyx_t_3 = (PyObject *) *__Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
-    if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
-    __Pyx_INCREF((PyObject*)__pyx_t_3);
+    if (unlikely(__pyx_v_array == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 30, __pyx_L1_error)
+    }
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_i);
+    __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_temp, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "nazo_rand/nazo_rand.pyx":31
  *         j = cy_uniform_int_variate(0, i)
  *         temp = array[i]
  *         array[i] = array[j]             # <<<<<<<<<<<<<<
  *         array[j] = temp
  * 
  */
-    __pyx_t_4 = __pyx_v_j;
-    __pyx_t_3 = (PyObject *) *__Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
-    if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
-    __Pyx_INCREF((PyObject*)__pyx_t_3);
-    __pyx_t_4 = __pyx_v_i;
-    __pyx_t_5 = __Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
-    __Pyx_XGOTREF(*__pyx_t_5);
-    __Pyx_INCREF(__pyx_t_3); __Pyx_XDECREF(*__pyx_t_5);
-    *__pyx_t_5 = __pyx_t_3;
-    __Pyx_XGIVEREF(*__pyx_t_5);
+    if (unlikely(__pyx_v_array == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 31, __pyx_L1_error)
+    }
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_j);
+    __Pyx_INCREF(__pyx_t_3);
+    if (unlikely(__pyx_v_array == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 31, __pyx_L1_error)
+    }
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_3, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "nazo_rand/nazo_rand.pyx":32
  *         temp = array[i]
  *         array[i] = array[j]
  *         array[j] = temp             # <<<<<<<<<<<<<<
  * 
- * def randbelow(a:int) -> int:
+ * 
  */
-    __pyx_t_4 = __pyx_v_j;
-    __pyx_t_5 = __Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
-    __Pyx_XGOTREF(*__pyx_t_5);
-    __Pyx_INCREF(__pyx_v_temp); __Pyx_XDECREF(*__pyx_t_5);
-    *__pyx_t_5 = __pyx_v_temp;
-    __Pyx_XGIVEREF(*__pyx_t_5);
+    if (unlikely(__pyx_v_array == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 32, __pyx_L1_error)
+    }
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_v_temp, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 32, __pyx_L1_error)
   }
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef object temp
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_WriteUnraisable("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  goto __pyx_L2;
   __pyx_L0:;
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-  __pyx_L2:;
   __Pyx_XDECREF(__pyx_v_temp);
   __Pyx_RefNannyFinishContext();
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
 static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_3shuffle = {"shuffle", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_3shuffle, METH_O, 0};
@@ -1848,73 +1749,53 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shuffle (wrapper)", 0);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject *)__pyx_v_array));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array) {
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
-  __Pyx_Buffer __pyx_pybuffer_array;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
-  __pyx_pybuffer_array.pybuffer.buf = NULL;
-  __pyx_pybuffer_array.refcount = 0;
-  __pyx_pybuffernd_array.data = NULL;
-  __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[0].suboffsets = __pyx_pybuffernd_array.rcbuffer->pybuffer.suboffsets[0];
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(((PyObject *)__pyx_v_array), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_AddTraceback("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  goto __pyx_L2;
   __pyx_L0:;
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-  __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":34
- *         array[j] = temp
+/* "nazo_rand/nazo_rand.pyx":35
+ * 
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
 /* Python wrapper */
@@ -1937,31 +1818,31 @@
   int64_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randbelow", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":35
+  /* "nazo_rand/nazo_rand.pyx":36
  * 
  * def randbelow(a:int) -> int:
  *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
  * def randint(a:int, b:int) -> int:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 35, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int64_t(Storm::random_below(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int64_t(Storm::random_below(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
- *         array[j] = temp
+  /* "nazo_rand/nazo_rand.pyx":35
+ * 
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
   /* function exit code */
@@ -1971,15 +1852,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":37
+/* "nazo_rand/nazo_rand.pyx":38
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
 
@@ -2014,32 +1895,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 38, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 38, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_a = values[0];
     __pyx_v_b = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 38, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6randint(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -2055,31 +1936,31 @@
   int64_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randint", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":38
+  /* "nazo_rand/nazo_rand.pyx":39
  * 
  * def randint(a:int, b:int) -> int:
  *     return cy_uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_b); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(__pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_b); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(__pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":38
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
 
@@ -2090,15 +1971,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":44
+/* "nazo_rand/nazo_rand.pyx":45
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
@@ -2110,39 +1991,39 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":45
+  /* "nazo_rand/nazo_rand.pyx":46
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):
  *     cdef Py_ssize_t index = cy_random_below(len(container))             # <<<<<<<<<<<<<<
  *     return container[index]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_t_1);
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":47
  * cpdef object random_choice(object container):
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":44
+  /* "nazo_rand/nazo_rand.pyx":45
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
@@ -2176,15 +2057,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2193,15 +2074,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":50
+/* "nazo_rand/nazo_rand.pyx":51
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
@@ -2218,51 +2099,51 @@
   int64_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":51
+  /* "nazo_rand/nazo_rand.pyx":52
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":52
+  /* "nazo_rand/nazo_rand.pyx":53
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_v_count;
     __pyx_t_3 = __pyx_t_1;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_7genexpr__pyx_v__ = __pyx_t_4;
       __pyx_t_5 = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_v_container_length);
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 52, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 53, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   } /* exit inner scope */
   __pyx_r = ((PyObject *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":50
+  /* "nazo_rand/nazo_rand.pyx":51
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
@@ -2309,32 +2190,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 50, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 51, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 51, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 51, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10random_choices(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2348,15 +2229,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2365,15 +2246,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":56
+/* "nazo_rand/nazo_rand.pyx":57
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2392,146 +2273,146 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":57
+  /* "nazo_rand/nazo_rand.pyx":58
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":59
+  /* "nazo_rand/nazo_rand.pyx":60
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count             # <<<<<<<<<<<<<<
  *     cdef list temp = list(container)
  * 
  */
-  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < __pyx_v_count; __pyx_temp++) {
       __Pyx_INCREF(Py_None);
       __Pyx_GIVEREF(Py_None);
       PyList_SET_ITEM(__pyx_t_2, __pyx_temp, Py_None);
     }
   }
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":60
+  /* "nazo_rand/nazo_rand.pyx":61
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  *     cdef list temp = list(container)             # <<<<<<<<<<<<<<
  * 
  *     if count > container_length:
  */
-  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_temp = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":62
+  /* "nazo_rand/nazo_rand.pyx":63
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   __pyx_t_3 = ((__pyx_v_count > __pyx_v_container_length) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "nazo_rand/nazo_rand.pyx":63
+    /* "nazo_rand/nazo_rand.pyx":64
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 63, __pyx_L1_error)
+    __PYX_ERR(0, 64, __pyx_L1_error)
 
-    /* "nazo_rand/nazo_rand.pyx":62
+    /* "nazo_rand/nazo_rand.pyx":63
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":65
+  /* "nazo_rand/nazo_rand.pyx":66
  *         raise ValueError("Sample larger than population")
  * 
  *     for i in range(count):             # <<<<<<<<<<<<<<
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  */
   __pyx_t_1 = __pyx_v_count;
   __pyx_t_4 = __pyx_t_1;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "nazo_rand/nazo_rand.pyx":66
+    /* "nazo_rand/nazo_rand.pyx":67
  * 
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)             # <<<<<<<<<<<<<<
  *         result[i] = temp[j]
  *         temp[j] = temp[i]
  */
     __pyx_v_j = Storm::uniform_int_variate(__pyx_v_i, (__pyx_v_container_length - 1));
 
-    /* "nazo_rand/nazo_rand.pyx":67
+    /* "nazo_rand/nazo_rand.pyx":68
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]             # <<<<<<<<<<<<<<
  *         temp[j] = temp[i]
  * 
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_j);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 67, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "nazo_rand/nazo_rand.pyx":68
+    /* "nazo_rand/nazo_rand.pyx":69
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  *         temp[j] = temp[i]             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
 
-  /* "nazo_rand/nazo_rand.pyx":70
+  /* "nazo_rand/nazo_rand.pyx":71
  *         temp[j] = temp[i]
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":56
+  /* "nazo_rand/nazo_rand.pyx":57
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2579,32 +2460,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 56, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 57, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 56, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 57, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 56, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 57, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_sample(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2618,15 +2499,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2635,15 +2516,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":72
+/* "nazo_rand/nazo_rand.pyx":73
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2662,56 +2543,56 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "nazo_rand/nazo_rand.pyx":73
+  /* "nazo_rand/nazo_rand.pyx":74
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_rand/nazo_rand.pyx":74
+    /* "nazo_rand/nazo_rand.pyx":75
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:
  *         stop, start = start, 0             # <<<<<<<<<<<<<<
  *     return random_range(start, stop, step)
  * 
  */
     __pyx_t_2 = __pyx_v_start;
     __pyx_t_3 = 0;
     __pyx_v_stop = __pyx_t_2;
     __pyx_v_start = __pyx_t_3;
 
-    /* "nazo_rand/nazo_rand.pyx":73
+    /* "nazo_rand/nazo_rand.pyx":74
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":75
+  /* "nazo_rand/nazo_rand.pyx":76
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":73
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2765,42 +2646,42 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_step);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
+      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
     } else {
       __pyx_v_stop = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
+      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
     } else {
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 72, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
@@ -2820,15 +2701,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
   __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2837,39 +2718,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":78
+/* "nazo_rand/nazo_rand.pyx":79
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":79
+  /* "nazo_rand/nazo_rand.pyx":80
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":79
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
@@ -2910,32 +2791,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 79, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 78, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 79, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
+    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 78, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 79, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_16random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -2949,15 +2830,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2966,36 +2847,36 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":82
+/* "nazo_rand/nazo_rand.pyx":83
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":83
+  /* "nazo_rand/nazo_rand.pyx":84
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":82
+  /* "nazo_rand/nazo_rand.pyx":83
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
@@ -3023,15 +2904,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3119,32 +3000,32 @@
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 64, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":63
+  /* "nazo_rand/nazo_rand.pyx":64
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "nazo_rand/nazo_rand.pyx":21
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
@@ -3152,114 +3033,114 @@
  * 
  */
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 21, __pyx_L1_error)
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef object temp
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":34
- *         array[j] = temp
+  /* "nazo_rand/nazo_rand.pyx":35
+ * 
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 35, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":38
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 38, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":44
+  /* "nazo_rand/nazo_rand.pyx":45
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 44, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":50
+  /* "nazo_rand/nazo_rand.pyx":51
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 51, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 51, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":56
+  /* "nazo_rand/nazo_rand.pyx":57
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 57, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 57, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":73
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 73, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 73, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":79
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 79, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":82
+  /* "nazo_rand/nazo_rand.pyx":83
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 82, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3562,129 +3443,129 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef object temp
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
- *         array[j] = temp
+  /* "nazo_rand/nazo_rand.pyx":35
+ * 
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_2) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":38
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_b, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_b, __pyx_n_u_int) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":44
+  /* "nazo_rand/nazo_rand.pyx":45
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":50
+  /* "nazo_rand/nazo_rand.pyx":51
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":56
+  /* "nazo_rand/nazo_rand.pyx":57
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":73
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":79
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":82
+  /* "nazo_rand/nazo_rand.pyx":83
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
@@ -3760,584 +3641,65 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* IsLittleEndian */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
-{
-  union {
-    uint32_t u32;
-    uint8_t u8[4];
-  } S;
-  S.u32 = 0x01020304;
-  return S.u8[0] == 4;
-}
-
-/* BufferFormatCheck */
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type) {
-  stack[0].field = &ctx->root;
-  stack[0].parent_offset = 0;
-  ctx->root.type = type;
-  ctx->root.name = "buffer dtype";
-  ctx->root.offset = 0;
-  ctx->head = stack;
-  ctx->head->field = &ctx->root;
-  ctx->fmt_offset = 0;
-  ctx->head->parent_offset = 0;
-  ctx->new_packmode = '@';
-  ctx->enc_packmode = '@';
-  ctx->new_count = 1;
-  ctx->enc_count = 0;
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  ctx->is_valid_array = 0;
-  ctx->struct_alignment = 0;
-  while (type->typegroup == 'S') {
-    ++ctx->head;
-    ctx->head->field = type->fields;
-    ctx->head->parent_offset = 0;
-    type = type->fields->type;
-  }
+/* SetItemInt */
+static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
+    int r;
+    if (!j) return -1;
+    r = PyObject_SetItem(o, j, v);
+    Py_DECREF(j);
+    return r;
 }
-static int __Pyx_BufFmt_ParseNumber(const char** ts) {
-    int count;
-    const char* t = *ts;
-    if (*t < '0' || *t > '9') {
-      return -1;
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
+                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
+            PyObject* old = PyList_GET_ITEM(o, n);
+            Py_INCREF(v);
+            PyList_SET_ITEM(o, n, v);
+            Py_DECREF(old);
+            return 1;
+        }
     } else {
-        count = *t++ - '0';
-        while (*t >= '0' && *t <= '9') {
-            count *= 10;
-            count += *t++ - '0';
-        }
-    }
-    *ts = t;
-    return count;
-}
-static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
-    int number = __Pyx_BufFmt_ParseNumber(ts);
-    if (number == -1)
-        PyErr_Format(PyExc_ValueError,\
-                     "Does not understand character buffer dtype format string ('%c')", **ts);
-    return number;
-}
-static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
-  PyErr_Format(PyExc_ValueError,
-               "Unexpected format string character: '%c'", ch);
-}
-static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
-  switch (ch) {
-    case '?': return "'bool'";
-    case 'c': return "'char'";
-    case 'b': return "'signed char'";
-    case 'B': return "'unsigned char'";
-    case 'h': return "'short'";
-    case 'H': return "'unsigned short'";
-    case 'i': return "'int'";
-    case 'I': return "'unsigned int'";
-    case 'l': return "'long'";
-    case 'L': return "'unsigned long'";
-    case 'q': return "'long long'";
-    case 'Q': return "'unsigned long long'";
-    case 'f': return (is_complex ? "'complex float'" : "'float'");
-    case 'd': return (is_complex ? "'complex double'" : "'double'");
-    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
-    case 'T': return "a struct";
-    case 'O': return "Python object";
-    case 'P': return "a pointer";
-    case 's': case 'p': return "a string";
-    case 0: return "end";
-    default: return "unparseable format string";
-  }
-}
-static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return 2;
-    case 'i': case 'I': case 'l': case 'L': return 4;
-    case 'q': case 'Q': return 8;
-    case 'f': return (is_complex ? 8 : 4);
-    case 'd': return (is_complex ? 16 : 8);
-    case 'g': {
-      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
-      return 0;
-    }
-    case 'O': case 'P': return sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(short);
-    case 'i': case 'I': return sizeof(int);
-    case 'l': case 'L': return sizeof(long);
-    #ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
-    #endif
-    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
-    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
-    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
-    case 'O': case 'P': return sizeof(void*);
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_ass_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return -1;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_ass_item(o, i, v);
+        }
     }
-  }
-}
-typedef struct { char c; short x; } __Pyx_st_short;
-typedef struct { char c; int x; } __Pyx_st_int;
-typedef struct { char c; long x; } __Pyx_st_long;
-typedef struct { char c; float x; } __Pyx_st_float;
-typedef struct { char c; double x; } __Pyx_st_double;
-typedef struct { char c; long double x; } __Pyx_st_longdouble;
-typedef struct { char c; void *x; } __Pyx_st_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
-#endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
+#else
+#if CYTHON_COMPILING_IN_PYPY
+    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
+#else
+    if (is_list || PySequence_Check(o))
 #endif
-    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
+    {
+        return PySequence_SetItem(o, i, v);
     }
-}
-/* These are for computing the padding at the end of the struct to align
-   on the first member of the struct. This will probably the same as above,
-   but we don't have any guarantees.
- */
-typedef struct { short x; char c; } __Pyx_pad_short;
-typedef struct { int x; char c; } __Pyx_pad_int;
-typedef struct { long x; char c; } __Pyx_pad_long;
-typedef struct { float x; char c; } __Pyx_pad_float;
-typedef struct { double x; char c; } __Pyx_pad_double;
-typedef struct { long double x; char c; } __Pyx_pad_longdouble;
-typedef struct { void *x; char c; } __Pyx_pad_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
-#endif
-    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
-  switch (ch) {
-    case 'c':
-        return 'H';
-    case 'b': case 'h': case 'i':
-    case 'l': case 'q': case 's': case 'p':
-        return 'I';
-    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
-        return 'U';
-    case 'f': case 'd': case 'g':
-        return (is_complex ? 'C' : 'R');
-    case 'O':
-        return 'O';
-    case 'P':
-        return 'P';
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-  }
-}
-static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
-  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
-    const char* expected;
-    const char* quote;
-    if (ctx->head == NULL) {
-      expected = "end";
-      quote = "";
-    } else {
-      expected = ctx->head->field->type->name;
-      quote = "'";
-    }
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected %s%s%s but got %s",
-                 quote, expected, quote,
-                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
-  } else {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_StructField* parent = (ctx->head - 1)->field;
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
-                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
-                 parent->type->name, field->name);
-  }
-}
-static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
-  char group;
-  size_t size, offset, arraysize = 1;
-  if (ctx->enc_type == 0) return 0;
-  if (ctx->head->field->type->arraysize[0]) {
-    int i, ndim = 0;
-    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
-        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
-        ndim = 1;
-        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
-            PyErr_Format(PyExc_ValueError,
-                         "Expected a dimension of size %zu, got %zu",
-                         ctx->head->field->type->arraysize[0], ctx->enc_count);
-            return -1;
-        }
-    }
-    if (!ctx->is_valid_array) {
-      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
-                   ctx->head->field->type->ndim, ndim);
-      return -1;
-    }
-    for (i = 0; i < ctx->head->field->type->ndim; i++) {
-      arraysize *= ctx->head->field->type->arraysize[i];
-    }
-    ctx->is_valid_array = 0;
-    ctx->enc_count = 1;
-  }
-  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
-  do {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_TypeInfo* type = field->type;
-    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
-      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
-    } else {
-      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
-    }
-    if (ctx->enc_packmode == '@') {
-      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
-      size_t align_mod_offset;
-      if (align_at == 0) return -1;
-      align_mod_offset = ctx->fmt_offset % align_at;
-      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
-      if (ctx->struct_alignment == 0)
-          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
-                                                                 ctx->is_complex);
-    }
-    if (type->size != size || type->typegroup != group) {
-      if (type->typegroup == 'C' && type->fields != NULL) {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        ++ctx->head;
-        ctx->head->field = type->fields;
-        ctx->head->parent_offset = parent_offset;
-        continue;
-      }
-      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
-      } else {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-      }
-    }
-    offset = ctx->head->parent_offset + field->offset;
-    if (ctx->fmt_offset != offset) {
-      PyErr_Format(PyExc_ValueError,
-                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
-                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
-      return -1;
-    }
-    ctx->fmt_offset += size;
-    if (arraysize)
-      ctx->fmt_offset += (arraysize - 1) * size;
-    --ctx->enc_count;
-    while (1) {
-      if (field == &ctx->root) {
-        ctx->head = NULL;
-        if (ctx->enc_count != 0) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-        }
-        break;
-      }
-      ctx->head->field = ++field;
-      if (field->type == NULL) {
-        --ctx->head;
-        field = ctx->head->field;
-        continue;
-      } else if (field->type->typegroup == 'S') {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        if (field->type->fields->type == NULL) continue;
-        field = field->type->fields;
-        ++ctx->head;
-        ctx->head->field = field;
-        ctx->head->parent_offset = parent_offset;
-        break;
-      } else {
-        break;
-      }
-    }
-  } while (ctx->enc_count);
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  return 0;
-}
-static PyObject *
-__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
-{
-    const char *ts = *tsp;
-    int i = 0, number, ndim;
-    ++ts;
-    if (ctx->new_count != 1) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Cannot handle repeated arrays in format string");
-        return NULL;
-    }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-    ndim = ctx->head->field->type->ndim;
-    while (*ts && *ts != ')') {
-        switch (*ts) {
-            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
-            default:  break;
-        }
-        number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
-                        "Expected a dimension of size %zu, got %d",
-                        ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
-                                "Expected a comma in format string, got '%c'", *ts);
-        if (*ts == ',') ts++;
-        i++;
-    }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
-                            ctx->head->field->type->ndim, i);
-    if (!*ts) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Unexpected end of format string, expected ')'");
-        return NULL;
-    }
-    ctx->is_valid_array = 1;
-    ctx->new_count = 1;
-    *tsp = ++ts;
-    return Py_None;
-}
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
-  int got_Z = 0;
-  while (1) {
-    switch(*ts) {
-      case 0:
-        if (ctx->enc_type != 0 && ctx->head == NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        if (ctx->head != NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        return ts;
-      case ' ':
-      case '\r':
-      case '\n':
-        ++ts;
-        break;
-      case '<':
-        if (!__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '>':
-      case '!':
-        if (__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '=':
-      case '@':
-      case '^':
-        ctx->new_packmode = *ts++;
-        break;
-      case 'T':
-        {
-          const char* ts_after_sub;
-          size_t i, struct_count = ctx->new_count;
-          size_t struct_alignment = ctx->struct_alignment;
-          ctx->new_count = 1;
-          ++ts;
-          if (*ts != '{') {
-            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
-            return NULL;
-          }
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          ctx->enc_count = 0;
-          ctx->struct_alignment = 0;
-          ++ts;
-          ts_after_sub = ts;
-          for (i = 0; i != struct_count; ++i) {
-            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
-            if (!ts_after_sub) return NULL;
-          }
-          ts = ts_after_sub;
-          if (struct_alignment) ctx->struct_alignment = struct_alignment;
-        }
-        break;
-      case '}':
-        {
-          size_t alignment = ctx->struct_alignment;
-          ++ts;
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          if (alignment && ctx->fmt_offset % alignment) {
-            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
-          }
-        }
-        return ts;
-      case 'x':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->fmt_offset += ctx->new_count;
-        ctx->new_count = 1;
-        ctx->enc_count = 0;
-        ctx->enc_type = 0;
-        ctx->enc_packmode = ctx->new_packmode;
-        ++ts;
-        break;
-      case 'Z':
-        got_Z = 1;
-        ++ts;
-        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
-          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
-          return NULL;
-        }
-        CYTHON_FALLTHROUGH;
-      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
-      case 'l': case 'L': case 'q': case 'Q':
-      case 'f': case 'd': case 'g':
-      case 'O': case 'p':
-        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
-            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
-          ctx->enc_count += ctx->new_count;
-          ctx->new_count = 1;
-          got_Z = 0;
-          ++ts;
-          break;
-        }
-        CYTHON_FALLTHROUGH;
-      case 's':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->enc_count = ctx->new_count;
-        ctx->enc_packmode = ctx->new_packmode;
-        ctx->enc_type = *ts;
-        ctx->is_complex = got_Z;
-        ++ts;
-        ctx->new_count = 1;
-        got_Z = 0;
-        break;
-      case ':':
-        ++ts;
-        while(*ts != ':') ++ts;
-        ++ts;
-        break;
-      case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
-        break;
-      default:
-        {
-          int number = __Pyx_BufFmt_ExpectNumber(&ts);
-          if (number == -1) return NULL;
-          ctx->new_count = (size_t)number;
-        }
-    }
-  }
-}
-
-/* BufferGetAndValidate */
-  static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
-  if (unlikely(info->buf == NULL)) return;
-  if (info->suboffsets == __Pyx_minusones) info->suboffsets = NULL;
-  __Pyx_ReleaseBuffer(info);
-}
-static void __Pyx_ZeroBuffer(Py_buffer* buf) {
-  buf->buf = NULL;
-  buf->obj = NULL;
-  buf->strides = __Pyx_zeros;
-  buf->shape = __Pyx_zeros;
-  buf->suboffsets = __Pyx_minusones;
-}
-static int __Pyx__GetBufferAndValidate(
-        Py_buffer* buf, PyObject* obj,  __Pyx_TypeInfo* dtype, int flags,
-        int nd, int cast, __Pyx_BufFmt_StackElem* stack)
-{
-  buf->buf = NULL;
-  if (unlikely(__Pyx_GetBuffer(obj, buf, flags) == -1)) {
-    __Pyx_ZeroBuffer(buf);
-    return -1;
-  }
-  if (unlikely(buf->ndim != nd)) {
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer has wrong number of dimensions (expected %d, got %d)",
-                 nd, buf->ndim);
-    goto fail;
-  }
-  if (!cast) {
-    __Pyx_BufFmt_Context ctx;
-    __Pyx_BufFmt_Init(&ctx, stack, dtype);
-    if (!__Pyx_BufFmt_CheckString(&ctx, buf->format)) goto fail;
-  }
-  if (unlikely((size_t)buf->itemsize != dtype->size)) {
-    PyErr_Format(PyExc_ValueError,
-      "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "d byte%s) does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "d byte%s)",
-      buf->itemsize, (buf->itemsize > 1) ? "s" : "",
-      dtype->name, (Py_ssize_t)dtype->size, (dtype->size > 1) ? "s" : "");
-    goto fail;
-  }
-  if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
-  return 0;
-fail:;
-  __Pyx_SafeReleaseBuffer(buf);
-  return -1;
+    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
-
-static CYTHON_INLINE void* __Pyx_BufPtrFull1d_imp(void* buf, Py_ssize_t i0, Py_ssize_t s0, Py_ssize_t o0) {
-  char* ptr = (char*)buf;
-ptr += s0 * i0;
-if (o0 >= 0) ptr = *((char**)ptr) + o0;
-
-return ptr;
-}
-  /* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -4353,15 +3715,15 @@
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* WriteUnraisableException */
-  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
                                   CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
                                   int full_traceback, CYTHON_UNUSED int nogil) {
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
@@ -4393,15 +3755,15 @@
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
 /* ArgTypeTest */
-  static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
@@ -4414,15 +3776,15 @@
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
 /* RaiseArgTupleInvalid */
-  static void __Pyx_RaiseArgtupleInvalid(
+static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
 {
     Py_ssize_t num_expected;
@@ -4440,29 +3802,29 @@
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* RaiseDoubleKeywords */
-  static void __Pyx_RaiseDoubleKeywordsError(
+static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
         "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
         #else
         "%s() got multiple values for keyword argument '%s'", func_name,
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
-  static int __Pyx_ParseOptionalKeywords(
+static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
@@ -4556,15 +3918,15 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* GetItemInt */
-  static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
@@ -4643,15 +4005,15 @@
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCall */
-  #if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
@@ -4663,15 +4025,15 @@
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* RaiseException */
-  #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
@@ -4821,65 +4183,16 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* SetItemInt */
-  static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
-    int r;
-    if (!j) return -1;
-    r = PyObject_SetItem(o, j, v);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
-                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
-            PyObject* old = PyList_GET_ITEM(o, n);
-            Py_INCREF(v);
-            PyList_SET_ITEM(o, n, v);
-            Py_DECREF(old);
-            return 1;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return -1;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_ass_item(o, i, v);
-        }
-    }
-#else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
-    {
-        return PySequence_SetItem(o, i, v);
-    }
-#endif
-    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
-}
-
 /* FetchCommonType */
-  static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
     cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
     if (cached_type) {
@@ -4910,15 +4223,15 @@
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
 /* CythonFunctionShared */
-  #include <structmember.h>
+#include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(op->func.m_ml->ml_doc);
@@ -5526,28 +4839,28 @@
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
 /* CythonFunction */
-  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
     PyObject *op = __Pyx_CyFunction_Init(
         PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
         ml, flags, qualname, closure, module, globals, code
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* PyDictVersioning */
-  #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
     PyObject **dictptr = NULL;
     Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
@@ -5565,15 +4878,15 @@
     if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
-  #ifndef CYTHON_CLINE_IN_TRACEBACK
+#ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
@@ -5607,15 +4920,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -5687,15 +5000,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-  #include "compile.h"
+#include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -5793,36 +5106,16 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-#if PY_MAJOR_VERSION < 3
-static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
-    if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
-    return -1;
-}
-static void __Pyx_ReleaseBuffer(Py_buffer *view) {
-    PyObject *obj = view->obj;
-    if (!obj) return;
-    if (PyObject_CheckBuffer(obj)) {
-        PyBuffer_Release(view);
-        return;
-    }
-    if ((0)) {}
-    view->obj = NULL;
-    Py_DECREF(obj);
-}
-#endif
-
-
-  /* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+/* CIntFromPyVerify */
+#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -5836,15 +5129,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
-  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6032,15 +5325,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6070,15 +5363,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6108,15 +5401,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
+static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6304,15 +5597,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int64_t");
     return (int64_t) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6342,15 +5635,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -6538,15 +5831,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* FastTypeChecks */
-  #if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
@@ -6638,15 +5931,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
+static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
     for (i = 0; i < 4; i++) {
         if (!ctversion[i]) {
@@ -6676,15 +5969,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* FunctionExport */
-  static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig) {
+static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(__pyx_m, (char *)"__pyx_capi__");
@@ -6713,15 +6006,15 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
```

### Comparing `nazo_rand-0.0.8/nazo_rand/nazo_rand.hpp` & `nazo_rand-0.0.9/nazo_rand/nazo_rand.hpp`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.8/nazo_rand/nazo_rand.pxd` & `nazo_rand-0.0.9/nazo_rand/nazo_rand.pxd`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.8/nazo_rand/nazo_rand.pyi` & `nazo_rand-0.0.9/nazo_rand/nazo_rand.pyi`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.8/nazo_rand/nazo_rand.pyx` & `nazo_rand-0.0.9/nazo_rand/nazo_rand.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 
 cdef inline int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
     return uniform_int_variate(a, b)
 
 cpdef int random_integer_noargs():
     return uniform_int_variate_noargs()
 
-cpdef void shuffle(list[object] array):
+cpdef void shuffle(list array):
     cdef int i, j
     cdef object temp
     cdef int length = len(array)
     for i in range(length - 1, 0, -1):
         j = cy_uniform_int_variate(0, i)
         temp = array[i]
         array[i] = array[j]
         array[j] = temp
 
+
 def randbelow(a:int) -> int:
     return random_below(a)
 
 def randint(a:int, b:int) -> int:
     return cy_uniform_int_variate(a, b)
```

### Comparing `nazo_rand-0.0.8/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.9/nazo_rand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nazo-rand
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nazo_rand
```

### Comparing `nazo_rand-0.0.8/setup.py` & `nazo_rand-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             "wraparound": False,
             "binding": True,
             "cdivision": True,
         },
     ),
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.8",
+    version="0.0.9",
     description="A fast random number generator for python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     package_data={
         "": [
             "nazo_rand/nazo_rand.pyi",
@@ -60,12 +60,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Cython",
         "Programming Language :: C++",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.8",
     packages=["nazo_rand"],
 )
```

