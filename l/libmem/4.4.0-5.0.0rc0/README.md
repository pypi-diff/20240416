# Comparing `tmp/libmem-4.4.0.tar.gz` & `tmp/libmem-5.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmem-4.4.0.tar", last modified: Wed Dec 13 16:40:13 2023, max compression
+gzip compressed data, was "libmem-5.0.0rc0.tar", last modified: Tue Apr 16 18:32:06 2024, max compression
```

## Comparing `libmem-4.4.0.tar` & `libmem-5.0.0rc0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-12-13 16:40:13.067062 libmem-4.4.0/
--rw-r--r--   0 user      (1000) user      (1000)       40 2023-12-08 20:51:07.000000 libmem-4.4.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)    10305 2023-12-13 16:40:13.063729 libmem-4.4.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     9774 2023-12-13 16:31:58.000000 libmem-4.4.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       99 2023-12-08 20:51:07.000000 libmem-4.4.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-12-13 16:40:13.067062 libmem-4.4.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1563 2023-12-13 16:31:58.000000 libmem-4.4.0/setup.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-12-13 16:40:13.063729 libmem-4.4.0/src/
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-12-13 16:40:13.063729 libmem-4.4.0/src/libmem-py/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-12-08 20:51:07.000000 libmem-4.4.0/src/libmem-py/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    39095 2023-12-08 20:51:07.000000 libmem-4.4.0/src/libmem-py/libmem-py.c
--rw-r--r--   0 user      (1000) user      (1000)    13553 2023-12-08 20:51:07.000000 libmem-4.4.0/src/libmem-py/types.h
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-12-13 16:40:13.063729 libmem-4.4.0/src/libmem.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    10305 2023-12-13 16:40:12.000000 libmem-4.4.0/src/libmem.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-12-13 16:40:13.000000 libmem-4.4.0/src/libmem.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-12-13 16:40:12.000000 libmem-4.4.0/src/libmem.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-12-13 16:40:12.000000 libmem-4.4.0/src/libmem.egg-info/top_level.txt
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/
+-rw-r--r--   0 user      (1000) user      (1000)       37 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    10546 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    10012 2024-04-16 18:29:37.000000 libmem-5.0.0rc0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       99 2024-04-10 14:57:23.000000 libmem-5.0.0rc0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-16 18:32:06.365788 libmem-5.0.0rc0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     4510 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/setup.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.363788 libmem-5.0.0rc0/src/
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.363788 libmem-5.0.0rc0/src/libmem/
+-rw-r--r--   0 user      (1000) user      (1000)     7967 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/__init__.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/src/libmem/_libmem/
+-rw-r--r--   0 user      (1000) user      (1000)    40715 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/_libmem/libmem-py.c
+-rw-r--r--   0 user      (1000) user      (1000)    13552 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/_libmem/types.h
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/src/libmem.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    10546 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      296 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       15 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/top_level.txt
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/tests/
+-rw-r--r--   0 user      (1000) user      (1000)    14338 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/tests/test_mock.py
+-rw-r--r--   0 user      (1000) user      (1000)     6846 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/tests/tests.py
```

### Comparing `libmem-4.4.0/PKG-INFO` & `libmem-5.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmem
-Version: 4.4.0
+Version: 5.0.0rc0
 Summary: Advanced Game Hacking Library (Windows/Linux/FreeBSD)
 Home-page: https://github.com/rdbo/libmem
 Author: rdbo
 Project-URL: Documentation, https://github.com/rdbo/libmem/blob/master/docs/DOCS.md
 Project-URL: Bug Tracker, https://github.com/rdbo/libmem/issues
 Project-URL: Discord Server, https://discord.com/invite/Qw8jsPD99X
 Keywords: gamehacking memory process hooking detouring hacking winapi linux freebsd
@@ -27,32 +27,35 @@
 NOTE: Submodules and external dependencies might have their own licenses! Check for other `LICENSE` files as well.
 
 ## Features
 - Cross Platform (Windows/Linux/FreeBSD)
 - Cross Architecture (x86/x64/ARM/ARM64)
 
 `libmem` can:
-- *Find Processes*
-- *Find Modules*
-- *Find Symbols*
-- *Read/Write/Set Memory*
-- *Allocate/Protect Memory*
-- *Scan Memory by Pattern/Signature*
-- *Hook/Unhook Functions*
-- *Assemble/Dissassemble Code (JIT)*
-- *Do VMT Hooking/Unhooking*
-- *Load/Unload Modules*
-- *Get Page Information*
-- *Enumerate Process Threads*
+- Find Processes
+- Find Modules
+- Find Symbols
+- Read/Write/Set Memory
+- Allocate/Protect Memory
+- Scan Memory by Pattern/Signature
+- Resolve pointer scans/pointer maps
+- Hook/Unhook Functions
+- Assemble/Dissassemble Code (JIT)
+- Do VMT Hooking/Unhooking
+- Load/Unload Modules
+- Get Page Information
+- Enumerate Process Threads
 
 ***And much more!***
 
 ## Examples
 
-For more examples and API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/DOCS.md)
+For the API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/README.md)
+
+For more examples, access the [examples directory](https://github.com/rdbo/libmem/blob/master/examples/README.md)
 
 ### C/C++
 ```c
 #include <libmem/libmem.h>
 
 int main()
 {
@@ -333,14 +336,16 @@
 LM_SetMemoryEx
 LM_ProtMemory
 LM_ProtMemoryEx
 LM_AllocMemory
 LM_AllocMemoryEx
 LM_FreeMemory
 LM_FreeMemoryEx
+LM_DeepPointer
+LM_DeepPointerEx
 
 LM_DataScan
 LM_DataScanEx
 LM_PatternScan
 LM_PatternScanEx
 LM_SigScan
 LM_SigScanEx
@@ -363,14 +368,17 @@
 LM_VmtHook
 LM_VmtUnhook
 LM_VmtGetOriginal
 LM_VmtReset
 LM_VmtFree
 ```
 
+## Contributing
+Read the file `CONTRIBUTING.md` in the root directory of this repository
+
 ## Projects
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)
```

### Comparing `libmem-4.4.0/README.md` & `libmem-5.0.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,35 @@
 NOTE: Submodules and external dependencies might have their own licenses! Check for other `LICENSE` files as well.
 
 ## Features
 - Cross Platform (Windows/Linux/FreeBSD)
 - Cross Architecture (x86/x64/ARM/ARM64)
 
 `libmem` can:
-- *Find Processes*
-- *Find Modules*
-- *Find Symbols*
-- *Read/Write/Set Memory*
-- *Allocate/Protect Memory*
-- *Scan Memory by Pattern/Signature*
-- *Hook/Unhook Functions*
-- *Assemble/Dissassemble Code (JIT)*
-- *Do VMT Hooking/Unhooking*
-- *Load/Unload Modules*
-- *Get Page Information*
-- *Enumerate Process Threads*
+- Find Processes
+- Find Modules
+- Find Symbols
+- Read/Write/Set Memory
+- Allocate/Protect Memory
+- Scan Memory by Pattern/Signature
+- Resolve pointer scans/pointer maps
+- Hook/Unhook Functions
+- Assemble/Dissassemble Code (JIT)
+- Do VMT Hooking/Unhooking
+- Load/Unload Modules
+- Get Page Information
+- Enumerate Process Threads
 
 ***And much more!***
 
 ## Examples
 
-For more examples and API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/DOCS.md)
+For the API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/README.md)
+
+For more examples, access the [examples directory](https://github.com/rdbo/libmem/blob/master/examples/README.md)
 
 ### C/C++
 ```c
 #include <libmem/libmem.h>
 
 int main()
 {
@@ -320,14 +323,16 @@
 LM_SetMemoryEx
 LM_ProtMemory
 LM_ProtMemoryEx
 LM_AllocMemory
 LM_AllocMemoryEx
 LM_FreeMemory
 LM_FreeMemoryEx
+LM_DeepPointer
+LM_DeepPointerEx
 
 LM_DataScan
 LM_DataScanEx
 LM_PatternScan
 LM_PatternScanEx
 LM_SigScan
 LM_SigScanEx
@@ -350,14 +355,17 @@
 LM_VmtHook
 LM_VmtUnhook
 LM_VmtGetOriginal
 LM_VmtReset
 LM_VmtFree
 ```
 
+## Contributing
+Read the file `CONTRIBUTING.md` in the root directory of this repository
+
 ## Projects
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)
```

### Comparing `libmem-4.4.0/src/libmem-py/libmem-py.c` & `libmem-5.0.0rc0/src/libmem/_libmem/libmem-py.c`

 * *Files 3% similar despite different names*

```diff
@@ -677,15 +677,15 @@
 py_LM_GetPage(PyObject *self,
 	      PyObject *args)
 {
 	lm_address_t address;
 	lm_page_t page;
 	py_lm_page_obj *pypage;
 
-	if (!PyArg_ParseTuple(args, "k", &address))
+	if (!PyArg_ParseTuple(args, "n", &address))
 		return NULL;
 
 	if (!LM_GetPage(address, &page))
 		return Py_BuildValue("");
 
 	pypage = (py_lm_page_obj *)PyObject_CallObject((PyObject *)&py_lm_page_t, NULL);
 	pypage->page = page;
@@ -701,15 +701,15 @@
 		PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t address;
 	lm_page_t page;
 	py_lm_page_obj *pypage;
 
-	if (!PyArg_ParseTuple(args, "Ok", &pyproc, &address))
+	if (!PyArg_ParseTuple(args, "On", &pyproc, &address))
 		return NULL;
 
 	if (!LM_GetPageEx(&pyproc->proc, address, &page))
 		return Py_BuildValue("");
 
 	pypage = (py_lm_page_obj *)PyObject_CallObject((PyObject *)&py_lm_page_t, NULL);
 	pypage->page = page;
@@ -725,15 +725,15 @@
 		 PyObject *args)
 {
 	lm_address_t src;
 	lm_size_t size;
 	lm_byte_t *dst;
 	PyObject *pybuf;
 
-	if (!PyArg_ParseTuple(args, "kk", &src, &size))
+	if (!PyArg_ParseTuple(args, "nn", &src, &size))
 		return NULL;
 
 	dst = LM_MALLOC(size);
 	if (!dst)
 		return Py_BuildValue("");
 
 	if (LM_ReadMemory(src, dst, size) == size) {
@@ -755,15 +755,15 @@
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t src;
 	lm_size_t size;
 	lm_byte_t *dst;
 	PyObject *pybuf;
 
-	if (!PyArg_ParseTuple(args, "Okk", &pyproc, &src, &size))
+	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &src, &size))
 		return NULL;
 
 	dst = LM_MALLOC(size);
 	if (!dst)
 		return Py_BuildValue("");
 
 	if (LM_ReadMemoryEx(&pyproc->proc, src, dst, size) == size) {
@@ -784,15 +784,15 @@
 		  PyObject *args)
 {
 	lm_address_t dst;
 	PyObject *pysrc;
 	lm_bytearr_t src;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "kY", &dst, &pysrc))
+	if (!PyArg_ParseTuple(args, "nY", &dst, &pysrc))
 		return NULL;
 
 	src = (lm_bytearr_t)PyByteArray_AsString(pysrc);
 	size = (lm_size_t)PyByteArray_Size(pysrc);
 
 	if (LM_WriteMemory(dst, src, size) != size)
 		Py_RETURN_FALSE;
@@ -808,15 +808,15 @@
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t dst;
 	PyObject *pysrc;
 	lm_bytearr_t src;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "OkY", &pyproc, &dst, &pysrc))
+	if (!PyArg_ParseTuple(args, "OnY", &pyproc, &dst, &pysrc))
 		return NULL;
 
 	src = (lm_bytearr_t)PyByteArray_AsString(pysrc);
 	size = (lm_size_t)PyByteArray_Size(pysrc);
 
 	if (LM_WriteMemoryEx(&pyproc->proc, dst, src, size) != size)
 		Py_RETURN_FALSE;
@@ -830,15 +830,15 @@
 py_LM_SetMemory(PyObject *self,
 		PyObject *args)
 {
 	lm_address_t dst;
 	lm_byte_t byte;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "kck", &dst, &byte, &size))
+	if (!PyArg_ParseTuple(args, "ncn", &dst, &byte, &size))
 		return NULL;
 
 	if (LM_SetMemory(dst, byte, size) != size)
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
@@ -850,15 +850,15 @@
 		  PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t dst;
 	lm_byte_t byte;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "kck", &pyproc, &dst, &byte, &size))
+	if (!PyArg_ParseTuple(args, "ncn", &pyproc, &dst, &byte, &size))
 		return NULL;
 
 	if (LM_SetMemoryEx(&pyproc->proc, dst, byte, size) != size)
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
@@ -871,15 +871,15 @@
 {
 	lm_address_t addr;
 	lm_size_t size;
 	py_lm_prot_obj *pyprot;
 	lm_prot_t oldprot;
 	py_lm_prot_obj *pyoldprot;
 
-	if (!PyArg_ParseTuple(args, "kkO", &addr, &size, &pyprot))
+	if (!PyArg_ParseTuple(args, "nnO", &addr, &size, &pyprot))
 		return NULL;
 
 	if (!LM_ProtMemory(addr, size, pyprot->prot, &oldprot))
 		return Py_BuildValue("");
 
 	pyoldprot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", oldprot);
 
@@ -895,15 +895,15 @@
 	py_lm_process_obj *pyproc;
 	lm_address_t addr;
 	lm_size_t size;
 	py_lm_prot_obj *pyprot;
 	lm_prot_t oldprot;
 	py_lm_prot_obj *pyoldprot;
 
-	if (!PyArg_ParseTuple(args, "OkkO", &pyproc, &addr, &size, &pyprot))
+	if (!PyArg_ParseTuple(args, "OnnO", &pyproc, &addr, &size, &pyprot))
 		return NULL;
 
 	if (!LM_ProtMemoryEx(&pyproc->proc, addr, size, pyprot->prot, &oldprot))
 		return Py_BuildValue("");
 
 	pyoldprot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", oldprot);
 
@@ -916,15 +916,15 @@
 py_LM_AllocMemory(PyObject *self,
 		  PyObject *args)
 {
 	lm_size_t size;
 	py_lm_prot_obj *pyprot;
 	lm_address_t alloc;
 
-	if (!PyArg_ParseTuple(args, "kO", &size, &pyprot))
+	if (!PyArg_ParseTuple(args, "nO", &size, &pyprot))
 		return NULL;
 
 
 	alloc = LM_AllocMemory(size, pyprot->prot);
 	if (alloc == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
@@ -938,15 +938,15 @@
 		    PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_size_t size;
 	py_lm_prot_obj *pyprot;
 	lm_address_t alloc;
 
-	if (!PyArg_ParseTuple(args, "OkO", &pyproc, &size, &pyprot))
+	if (!PyArg_ParseTuple(args, "OnO", &pyproc, &size, &pyprot))
 		return NULL;
 
 
 	alloc = LM_AllocMemoryEx(&pyproc->proc, size, pyprot->prot);
 	if (alloc == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
@@ -958,15 +958,15 @@
 static PyObject *
 py_LM_FreeMemory(PyObject *self,
 		 PyObject *args)
 {
 	lm_address_t alloc;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "kk", &alloc, &size))
+	if (!PyArg_ParseTuple(args, "nn", &alloc, &size))
 		return NULL;
 
 
 	if (!LM_FreeMemory(alloc, size))
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
@@ -978,38 +978,115 @@
 py_LM_FreeMemoryEx(PyObject *self,
 		   PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t alloc;
 	lm_size_t size;
 
-	if (!PyArg_ParseTuple(args, "Okk", &pyproc, &alloc, &size))
+	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &alloc, &size))
 		return NULL;
 
 
 	if (!LM_FreeMemoryEx(&pyproc->proc, alloc, size))
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
 
 /****************************************/
 
 static PyObject *
+py_LM_DeepPointer(PyObject *self,
+		  PyObject *args)
+{
+	lm_address_t  base;
+	PyObject     *pyoffsets;
+	lm_address_t *offsets;
+	lm_size_t     noffsets;
+	lm_address_t  pointer;
+	lm_size_t     i;
+
+	if (!PyArg_ParseTuple(args, "nO", &base, &pyoffsets))
+		return NULL;
+
+	noffsets = PyList_Size(pyoffsets);
+	if (noffsets == 0)
+		return PyLong_FromSize_t(base);
+
+	offsets = LM_CALLOC(sizeof(lm_address_t), noffsets);
+	if (!offsets)
+		return NULL;
+
+	for (i = 0; i < noffsets; ++i) {
+		offsets[i] = (lm_address_t)PyLong_AsSize_t(PyList_GetItem(pyoffsets, i));
+	}
+
+	pointer = LM_DeepPointer(base, offsets, noffsets);
+
+	LM_FREE(offsets);
+
+	if (pointer == LM_ADDRESS_BAD)
+		return Py_BuildValue("");
+
+	return PyLong_FromSize_t(pointer);
+}
+
+/****************************************/
+
+static PyObject *
+py_LM_DeepPointerEx(PyObject *self,
+		    PyObject *args)
+{
+	py_lm_process_obj *pyproc;
+	lm_address_t  base;
+	PyObject     *pyoffsets;
+	lm_address_t *offsets;
+	lm_size_t     noffsets;
+	lm_address_t  pointer;
+	lm_size_t     i;
+
+	if (!PyArg_ParseTuple(args, "OnO", &pyproc, &base, &pyoffsets))
+		return NULL;
+
+	noffsets = PyList_Size(pyoffsets);
+	if (noffsets == 0)
+		return PyLong_FromSize_t(base);
+
+	offsets = LM_CALLOC(sizeof(lm_address_t), noffsets);
+	if (!offsets)
+		return NULL;
+
+	for (i = 0; i < noffsets; ++i) {
+		offsets[i] = (lm_address_t)PyLong_AsSize_t(PyList_GetItem(pyoffsets, i));
+	}
+
+	pointer = LM_DeepPointerEx(&pyproc->proc, base, offsets, noffsets);
+
+	LM_FREE(offsets);
+
+	if (pointer == LM_ADDRESS_BAD)
+		return Py_BuildValue("");
+
+	return PyLong_FromSize_t(pointer);
+}
+
+/****************************************/
+
+static PyObject *
 py_LM_DataScan(PyObject *self,
 	       PyObject *args)
 {
 	PyObject *pydata;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_bytearr_t data;
 	lm_size_t size;
 	lm_address_t scan_match;
 
-	if (!PyArg_ParseTuple(args, "Ykk", &pydata, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "Ynn", &pydata, &addr, &scansize))
 		return NULL;
 
 	data = (lm_bytearr_t)PyByteArray_AsString(pydata);
 	size = (lm_size_t)PyByteArray_Size(pydata);
 
 	scan_match = LM_DataScan(data, size, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
@@ -1028,15 +1105,15 @@
 	PyObject *pydata;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_bytearr_t data;
 	lm_size_t size;
 	lm_address_t scan_match;
 
-	if (!PyArg_ParseTuple(args, "OYkk", &pyproc, &pydata, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "OYnn", &pyproc, &pydata, &addr, &scansize))
 		return NULL;
 
 	data = (lm_bytearr_t)PyByteArray_AsString(pydata);
 	size = (lm_size_t)PyByteArray_Size(pydata);
 
 	scan_match = LM_DataScanEx(&pyproc->proc, data, size, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
@@ -1055,18 +1132,18 @@
 	lm_char_t *mask;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_bytearr_t pattern;
 	lm_address_t scan_match;
 
 #	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Yukk", &pypattern, &mask, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "Yunn", &pypattern, &mask, &addr, &scansize))
 		return NULL;
 #	else
-	if (!PyArg_ParseTuple(args, "Yskk", &pypattern, &mask, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "Ysnn", &pypattern, &mask, &addr, &scansize))
 		return NULL;
 #	endif
 
 	pattern = (lm_bytearr_t)PyByteArray_AsString(pypattern);
 
 	scan_match = LM_PatternScan(pattern, mask, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
@@ -1086,18 +1163,18 @@
 	lm_char_t *mask;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_bytearr_t pattern;
 	lm_address_t scan_match;
 
 #	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "OYukk", &pyproc, &pypattern, &mask, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "OYunn", &pyproc, &pypattern, &mask, &addr, &scansize))
 		return NULL;
 #	else
-	if (!PyArg_ParseTuple(args, "OYskk", &pyproc, &pypattern, &mask, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "OYsnn", &pyproc, &pypattern, &mask, &addr, &scansize))
 		return NULL;
 #	endif
 
 	pattern = (lm_bytearr_t)PyByteArray_AsString(pypattern);
 
 	scan_match = LM_PatternScanEx(&pyproc->proc, pattern, mask, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
@@ -1114,18 +1191,18 @@
 {
 	lm_char_t *sig;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_address_t scan_match;
 
 #	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "ukk", &sig, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "unn", &sig, &addr, &scansize))
 		return NULL;
 #	else
-	if (!PyArg_ParseTuple(args, "skk", &sig, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "snn", &sig, &addr, &scansize))
 		return NULL;
 #	endif
 
 	scan_match = LM_SigScan(sig, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
@@ -1141,18 +1218,18 @@
 	py_lm_process_obj *pyproc;
 	lm_char_t *sig;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_address_t scan_match;
 
 #	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Oukk", &pyproc, &sig, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "Ounn", &pyproc, &sig, &addr, &scansize))
 		return NULL;
 #	else
-	if (!PyArg_ParseTuple(args, "Oskk", &pyproc, &sig, &addr, &scansize))
+	if (!PyArg_ParseTuple(args, "Osnn", &pyproc, &sig, &addr, &scansize))
 		return NULL;
 #	endif
 
 	scan_match = LM_SigScanEx(&pyproc->proc, sig, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
@@ -1166,87 +1243,79 @@
 	       PyObject *args)
 {
 	lm_address_t from;
 	lm_address_t to;
 	lm_address_t trampoline;
 	lm_size_t    size;
 
-	if (!PyArg_ParseTuple(args, "kk", &from, &to))
+	if (!PyArg_ParseTuple(args, "nn", &from, &to))
 		return NULL;
 
 	size = LM_HookCode(from, to, &trampoline);
 	if (!size)
 		return Py_BuildValue("");
 
-	return Py_BuildValue("(kk)", trampoline, size);
+	return Py_BuildValue("(nn)", trampoline, size);
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_HookCodeEx(PyObject *self,
 		 PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t from;
 	lm_address_t to;
 	lm_address_t trampoline;
 	lm_size_t    size;
 
-	if (!PyArg_ParseTuple(args, "Okk", &pyproc, &from, &to))
+	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &from, &to))
 		return NULL;
 
 	size = LM_HookCodeEx(&pyproc->proc, from, to, &trampoline);
 	if (!size)
 		return Py_BuildValue("");
 
-	return Py_BuildValue("(kk)", trampoline, size);
+	return Py_BuildValue("(nn)", trampoline, size);
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_UnhookCode(PyObject *self,
 		 PyObject *args)
 {
 	lm_address_t from;
-	PyObject *pytrampoline;
 	lm_address_t trampoline;
 	lm_size_t    size;
 
-	if (!PyArg_ParseTuple(args, "k(kk)", &from, &pytrampoline))
+	if (!PyArg_ParseTuple(args, "n(nn)", &from, &trampoline, &size))
 		return NULL;
 
-	trampoline = (lm_address_t)PyLong_AsSize_t(PyTuple_GetItem(pytrampoline, 0));
-	size = (lm_size_t)PyLong_AsSize_t(PyTuple_GetItem(pytrampoline, 1));
-
 	if (!LM_UnhookCode(from, trampoline, size))
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_UnhookCodeEx(PyObject *self,
 		   PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t from;
-	PyObject *pytrampoline;
 	lm_address_t trampoline;
 	lm_size_t    size;
 
-	if (!PyArg_ParseTuple(args, "Ok(kk)", &pyproc, &from, &pytrampoline))
+	if (!PyArg_ParseTuple(args, "On(nn)", &pyproc, &from, &trampoline, &size))
 		return NULL;
 
-	trampoline = (lm_address_t)PyLong_AsSize_t(PyTuple_GetItem(pytrampoline, 0));
-	size = (lm_size_t)PyLong_AsSize_t(PyTuple_GetItem(pytrampoline, 1));
-
 	if (!LM_UnhookCodeEx(&pyproc->proc, from, trampoline, size))
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
 
 /****************************************/
@@ -1280,15 +1349,15 @@
 	lm_cstring_t code;
 	lm_size_t bits;
 	lm_address_t runtime_addr;
 	lm_bytearr_t codebuf;
 	lm_size_t codelen;
 	PyObject *pycodebuf;
 
-	if (!PyArg_ParseTuple(args, "skk", &code, &bits, &runtime_addr))
+	if (!PyArg_ParseTuple(args, "snn", &code, &bits, &runtime_addr))
 		return NULL;
 
 	codelen = LM_AssembleEx(code, bits, runtime_addr, &codebuf);
 	if (!codelen)
 		return Py_BuildValue("");
 
 	pycodebuf = PyByteArray_FromStringAndSize((const char *)codebuf, codelen);
@@ -1304,15 +1373,15 @@
 py_LM_Disassemble(PyObject *self,
 		  PyObject *args)
 {
 	lm_address_t code;
 	lm_inst_t inst;
 	py_lm_inst_obj *pyinst;
 
-	if (!PyArg_ParseTuple(args, "k", &code))
+	if (!PyArg_ParseTuple(args, "n", &code))
 		return NULL;
 
 	if (!LM_Disassemble(code, &inst))
 		return Py_BuildValue("");
 
 	pyinst = (py_lm_inst_obj *)PyObject_CallObject((PyObject *)&py_lm_inst_t, NULL);
 	pyinst->inst = inst;
@@ -1333,15 +1402,15 @@
 	lm_address_t runtime_addr;
 	lm_inst_t *insts;
 	lm_size_t inst_count;
 	PyObject *pyinsts;
 	lm_size_t i;
 	py_lm_inst_obj *pyinst;
 
-	if (!PyArg_ParseTuple(args, "kkkkk", &code, &bits, &size, &count, &runtime_addr))
+	if (!PyArg_ParseTuple(args, "nnnnn", &code, &bits, &size, &count, &runtime_addr))
 		return NULL;
 
 	inst_count = LM_DisassembleEx(code, bits, size, count, runtime_addr, &insts);
 	if (!inst_count)
 		return Py_BuildValue("");
 
 	pyinsts = PyList_New((Py_ssize_t)inst_count);
@@ -1362,15 +1431,15 @@
 py_LM_CodeLength(PyObject *self,
 		 PyObject *args)
 {
 	lm_address_t code;
 	lm_size_t minlength;
 	lm_size_t aligned_length;
 
-	if (!PyArg_ParseTuple(args, "kk", &code, &minlength))
+	if (!PyArg_ParseTuple(args, "nn", &code, &minlength))
 		return NULL;
 
 	aligned_length = LM_CodeLength(code, minlength);
 	if (!aligned_length)
 		return Py_BuildValue("");
 
 	return (PyObject *)PyLong_FromSize_t(aligned_length);
@@ -1383,15 +1452,15 @@
 		   PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t code;
 	lm_size_t minlength;
 	lm_size_t aligned_length;
 
-	if (!PyArg_ParseTuple(args, "Okk", &pyproc, &code, &minlength))
+	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &code, &minlength))
 		return NULL;
 
 	aligned_length = LM_CodeLengthEx(&pyproc->proc, code, minlength);
 	if (!aligned_length)
 		return Py_BuildValue("");
 
 	return (PyObject *)PyLong_FromSize_t(aligned_length);
@@ -1441,14 +1510,16 @@
 	{ "LM_SetMemoryEx", py_LM_SetMemoryEx, METH_VARARGS, "Set memory to a byte in a remote process" },
 	{ "LM_ProtMemory", py_LM_ProtMemory, METH_VARARGS, "Change memory protection flags of a region in the current process" },
 	{ "LM_ProtMemoryEx", py_LM_ProtMemoryEx, METH_VARARGS, "Change memory protection flags of a region in a remote process" },
 	{ "LM_AllocMemory", py_LM_AllocMemory, METH_VARARGS, "Allocate memory in the current process" },
 	{ "LM_AllocMemoryEx", py_LM_AllocMemoryEx, METH_VARARGS, "Allocate memory in a remote process" },
 	{ "LM_FreeMemory", py_LM_FreeMemory, METH_VARARGS, "Free memory in the current process" },
 	{ "LM_FreeMemoryEx", py_LM_FreeMemoryEx, METH_VARARGS, "Free memory in a remote process" },
+	{ "LM_DeepPointer", py_LM_DeepPointer, METH_VARARGS, "Dereference a deep pointer in the current process, usually result of a pointer map or pointer scan" },
+	{ "LM_DeepPointerEx", py_LM_DeepPointerEx, METH_VARARGS, "Dereference a deep pointer in a remote process, usually result of a pointer map or pointer scan" },
 	/****************************************/
 	{ "LM_DataScan", py_LM_DataScan, METH_VARARGS, "Search for a byte array in the current process" },
 	{ "LM_DataScanEx", py_LM_DataScanEx, METH_VARARGS, "Search for a byte array in a remote process" },
 	{ "LM_PatternScan", py_LM_PatternScan, METH_VARARGS, "Search for a byte pattern with a mask filter in the current process" },
 	{ "LM_PatternScanEx", py_LM_PatternScanEx, METH_VARARGS, "Search for a byte pattern with a mask filter in a remote process" },
 	{ "LM_SigScan", py_LM_SigScan, METH_VARARGS, "Search for a byte signature that can contain filters in the current process" },
 	{ "LM_SigScanEx", py_LM_SigScanEx, METH_VARARGS, "Search for a byte signature that can contain filters in a remote process" },
@@ -1465,22 +1536,22 @@
 	{ "LM_CodeLength", py_LM_CodeLength, METH_VARARGS, "Get the minimum instruction aligned length for a code region in the current process" },
 	{ "LM_CodeLengthEx", py_LM_CodeLengthEx, METH_VARARGS, "Get the minimum instruction aligned length for a code region in a remote process" },
 	{ NULL, NULL, 0, NULL }
 };
 
 static PyModuleDef libmem_mod = {
 	PyModuleDef_HEAD_INIT,
-	"libmem",
+	"_libmem",
 	NULL,
 	-1,
 	libmem_methods
 };
 
 PyMODINIT_FUNC
-PyInit_libmem(void)
+PyInit__libmem(void)
 {
 	PyObject *pymod;
 	PyObject *global; /* used in the DECL_GLOBAL macro */
 
 	if (PyType_Ready(&py_lm_process_t) < 0)
 		goto ERR_PYMOD;
```

### Comparing `libmem-4.4.0/src/libmem-py/types.h` & `libmem-5.0.0rc0/src/libmem/_libmem/types.h`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #ifndef LIBMEM_TYPES_H
 #define LIBMEM_TYPES_H
 
 #include <libmem/libmem.h>
 #include <Python.h>
 #include <structmember.h>
 
-#define T_SIZE T_ULONG
+#define T_SIZE T_PYSSIZET
 
 /* lm_process_t */
 typedef struct {
 	PyObject_HEAD
 	lm_process_t proc;
 } py_lm_process_obj;
 
@@ -382,15 +382,15 @@
 	.tp_getset = py_lm_inst_accessors,
 	.tp_str = py_lm_inst_str,
 	.tp_repr = py_lm_inst_str
 };
 
 /****************************************/
 
-/* lm_process_t */
+/* lm_vmt_t */
 typedef struct {
 	PyObject_HEAD
 	lm_vmt_t vmt;
 } py_lm_vmt_obj;
 
 PyObject *
 py_lm_vmt_str(PyObject *self)
```

### Comparing `libmem-4.4.0/src/libmem.egg-info/PKG-INFO` & `libmem-5.0.0rc0/src/libmem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmem
-Version: 4.4.0
+Version: 5.0.0rc0
 Summary: Advanced Game Hacking Library (Windows/Linux/FreeBSD)
 Home-page: https://github.com/rdbo/libmem
 Author: rdbo
 Project-URL: Documentation, https://github.com/rdbo/libmem/blob/master/docs/DOCS.md
 Project-URL: Bug Tracker, https://github.com/rdbo/libmem/issues
 Project-URL: Discord Server, https://discord.com/invite/Qw8jsPD99X
 Keywords: gamehacking memory process hooking detouring hacking winapi linux freebsd
@@ -27,32 +27,35 @@
 NOTE: Submodules and external dependencies might have their own licenses! Check for other `LICENSE` files as well.
 
 ## Features
 - Cross Platform (Windows/Linux/FreeBSD)
 - Cross Architecture (x86/x64/ARM/ARM64)
 
 `libmem` can:
-- *Find Processes*
-- *Find Modules*
-- *Find Symbols*
-- *Read/Write/Set Memory*
-- *Allocate/Protect Memory*
-- *Scan Memory by Pattern/Signature*
-- *Hook/Unhook Functions*
-- *Assemble/Dissassemble Code (JIT)*
-- *Do VMT Hooking/Unhooking*
-- *Load/Unload Modules*
-- *Get Page Information*
-- *Enumerate Process Threads*
+- Find Processes
+- Find Modules
+- Find Symbols
+- Read/Write/Set Memory
+- Allocate/Protect Memory
+- Scan Memory by Pattern/Signature
+- Resolve pointer scans/pointer maps
+- Hook/Unhook Functions
+- Assemble/Dissassemble Code (JIT)
+- Do VMT Hooking/Unhooking
+- Load/Unload Modules
+- Get Page Information
+- Enumerate Process Threads
 
 ***And much more!***
 
 ## Examples
 
-For more examples and API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/DOCS.md)
+For the API manual, access the [documentation](https://github.com/rdbo/libmem/blob/master/docs/README.md)
+
+For more examples, access the [examples directory](https://github.com/rdbo/libmem/blob/master/examples/README.md)
 
 ### C/C++
 ```c
 #include <libmem/libmem.h>
 
 int main()
 {
@@ -333,14 +336,16 @@
 LM_SetMemoryEx
 LM_ProtMemory
 LM_ProtMemoryEx
 LM_AllocMemory
 LM_AllocMemoryEx
 LM_FreeMemory
 LM_FreeMemoryEx
+LM_DeepPointer
+LM_DeepPointerEx
 
 LM_DataScan
 LM_DataScanEx
 LM_PatternScan
 LM_PatternScanEx
 LM_SigScan
 LM_SigScanEx
@@ -363,14 +368,17 @@
 LM_VmtHook
 LM_VmtUnhook
 LM_VmtGetOriginal
 LM_VmtReset
 LM_VmtFree
 ```
 
+## Contributing
+Read the file `CONTRIBUTING.md` in the root directory of this repository
+
 ## Projects
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)
```

