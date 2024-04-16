# Comparing `tmp/revizor_fuzzer-1.2.3.tar.gz` & `tmp/revizor_fuzzer-1.2.4.tar.gz`

## Comparing `revizor_fuzzer-1.2.3.tar` & `revizor_fuzzer-1.2.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.editorconfig
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.gitmodules
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.sync-exclude.lst
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/Makefile
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/SECURITY.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/mkdocs.yml
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/analyser.py
--rwxr-xr-x   0        0        0     8150 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/cli.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/config.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/coverage.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/executor.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/factory.py
--rw-r--r--   0        0        0    15571 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/fuzzer.py
--rw-r--r--   0        0        0    24707 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/generator.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/input_generator.py
--rw-r--r--   0        0        0    26042 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/interfaces.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/isa_loader.py
--rw-r--r--   0        0        0    35965 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/model.py
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/postprocessor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/py.typed
--rw-r--r--   0        0        0    40667 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/unicorn.pyi
--rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/__init__.py
--rwxr-xr-x   0        0        0    10643 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/get_spec.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_config.py
--rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_executor.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_fuzzer.py
--rw-r--r--   0        0        0    37970 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_generator.py
--rw-r--r--   0        0        0    32893 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_model.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/revizor/x86/x86_target_desc.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/AUTHORS
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/LICENSE
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/README.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/.editorconfig
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/.gitmodules
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/.sync-exclude.lst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/Makefile
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/SECURITY.md
+-rw-r--r--   0        0        0  1039705 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/base.json
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/mkdocs.yml
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/analyser.py
+-rwxr-xr-x   0        0        0     8150 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/cli.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/config.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/coverage.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/executor.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/factory.py
+-rw-r--r--   0        0        0    15571 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/fuzzer.py
+-rw-r--r--   0        0        0    25071 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/generator.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/input_generator.py
+-rw-r--r--   0        0        0    26066 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/interfaces.py
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/isa_loader.py
+-rw-r--r--   0        0        0    35965 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/model.py
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/postprocessor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/py.typed
+-rw-r--r--   0        0        0    40667 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/unicorn.pyi
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/__init__.py
+-rwxr-xr-x   0        0        0    10744 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/get_spec.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_config.py
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_executor.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_fuzzer.py
+-rw-r--r--   0        0        0    37970 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_generator.py
+-rw-r--r--   0        0        0    32893 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_model.py
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/revizor/x86/x86_target_desc.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/AUTHORS
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/LICENSE
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    12211 2020-02-02 00:00:00.000000 revizor_fuzzer-1.2.4/PKG-INFO
```

### Comparing `revizor_fuzzer-1.2.3/.editorconfig` & `revizor_fuzzer-1.2.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/CONTRIBUTING.md` & `revizor_fuzzer-1.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/SECURITY.md` & `revizor_fuzzer-1.2.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/mkdocs.yml` & `revizor_fuzzer-1.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/analyser.py` & `revizor_fuzzer-1.2.4/revizor/analyser.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/cli.py` & `revizor_fuzzer-1.2.4/revizor/cli.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/config.py` & `revizor_fuzzer-1.2.4/revizor/config.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/coverage.py` & `revizor_fuzzer-1.2.4/revizor/coverage.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/factory.py` & `revizor_fuzzer-1.2.4/revizor/factory.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/fuzzer.py` & `revizor_fuzzer-1.2.4/revizor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/generator.py` & `revizor_fuzzer-1.2.4/revizor/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     msg += line
                 else:
                     parsed = lines[int(line_num_str.group(1)) - 1]
                     msg += f"\n  Line {line}\n    (the line was parsed as {parsed})"
             return msg
 
         try:
-            out = run(f"as {asm_file} -o {bin_file}", shell=True, check=True, capture_output=True)
+            out = run(f"/home/t-oleksenkoo/bin/binutils-gdb/gas/as-new {asm_file} -o {bin_file}", shell=True, check=True, capture_output=True)
         except CalledProcessError as e:
             error_msg = e.stderr.decode()
             if "Assembler messages:" in error_msg:
                 print(pretty_error_msg(error_msg))
             else:
                 print(error_msg)
             raise e
@@ -494,29 +494,40 @@
         if spec.values:
             address_reg = random.choice(spec.values)
         else:
             address_reg = random.choice(self.target_desc.registers[64])
         return MemoryOperand(address_reg, spec.width, spec.src, spec.dest)
 
     def generate_imm_operand(self, spec: OperandSpec, _: Instruction) -> Operand:
+        # generate bitmask
+        if spec.values and spec.values[0] == "bitmask":
+            # FIXME: this implementation always returns the same bitmask
+            # make it random
+            value = str(pow(2, spec.width) - 2)
+            return ImmediateOperand(value, spec.width)
+
+        # generate from a predefined range
         if spec.values:
-            if spec.values[0] == "bitmask":
-                # FIXME: this implementation always returns the same bitmask
-                # make it random
-                value = str(pow(2, spec.width) - 2)
-            else:
-                assert "[" in spec.values[0], spec.values
-                range_ = spec.values[0][1:-1].split("-")
-                if range_[0] == "":
-                    range_ = range_[1:]
-                    range_[0] = "-" + range_[0]
-                assert len(range_) == 2
-                value = str(random.randint(int(range_[0]), int(range_[1])))
+            assert "[" in spec.values[0], spec.values
+            range_ = spec.values[0][1:-1].split("-")
+            if range_[0] == "":
+                range_ = range_[1:]
+                range_[0] = "-" + range_[0]
+            assert len(range_) == 2
+            value = str(random.randint(int(range_[0]), int(range_[1])))
+            ImmediateOperand(value, spec.width)
+
+        # generate from width
+        if spec.signed:
+            range_min = pow(2, spec.width - 1) * -1
+            range_max = pow(2, spec.width - 1) - 1
         else:
-            value = str(random.randint(pow(2, spec.width - 1) * -1, pow(2, spec.width - 1) - 1))
+            range_min = 0
+            range_max = pow(2, spec.width) - 1
+        value = str(random.randint(range_min, range_max))
         return ImmediateOperand(value, spec.width)
 
     def generate_label_operand(self, spec: OperandSpec, parent: Instruction) -> Operand:
         return LabelOperand("")  # the actual label will be set in add_terminators_in_function
 
     def generate_agen_operand(self, spec: OperandSpec, __: Instruction) -> Operand:
         n_operands = random.randint(1, 3)
```

### Comparing `revizor_fuzzer-1.2.3/revizor/input_generator.py` & `revizor_fuzzer-1.2.4/revizor/input_generator.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/interfaces.py` & `revizor_fuzzer-1.2.4/revizor/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         return str(self._name_)
 
 
 class OperandSpec:
     values: List[str]
     type: OT
     width: int
+    signed: bool = True
     src: bool
     dest: bool
 
     # certain operand values have special handling (e.g., separate opcode when RAX is a destination)
     # magic_value attribute indicates a specification for this special value
     magic_value: bool = False
```

### Comparing `revizor_fuzzer-1.2.3/revizor/isa_loader.py` & `revizor_fuzzer-1.2.4/revizor/isa_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     def parse_operand(self, op: Dict, parent: InstructionSpec) -> OperandSpec:
         op_type = self.ot_str_to_enum[op["type_"]]
         op_values = op.get("values", [])
         if op_type == "REG":
             op_values = sorted(op_values)
         spec = OperandSpec(op_values, op_type, op["src"], op["dest"])
         spec.width = op["width"]
+        spec.signed = op.get("signed", True)
 
         if op_type == OT.MEM:
             parent.has_mem_operand = True
             if spec.dest:
                 parent.has_write = True
 
         return spec
```

### Comparing `revizor_fuzzer-1.2.3/revizor/model.py` & `revizor_fuzzer-1.2.4/revizor/model.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/postprocessor.py` & `revizor_fuzzer-1.2.4/revizor/postprocessor.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/unicorn.pyi` & `revizor_fuzzer-1.2.4/revizor/unicorn.pyi`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/util.py` & `revizor_fuzzer-1.2.4/revizor/util.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/get_spec.py` & `revizor_fuzzer-1.2.4/revizor/x86/get_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from xml.etree import ElementTree as ET
 
 
 class OperandSpec:
     values: List[str]
     type_: str
     width: int
+    signed: bool = True
     comment: str
     src: bool = False
     dest: bool = False
     magic: bool = False
 
     def to_json(self) -> str:
         return json.dumps(self, default=vars)
@@ -213,14 +214,16 @@
         if op.attrib.get('implicit', '0') == '1':
             spec.values = [op.text]
         else:
             spec.values = []
         spec.src = True
         spec.dest = False
         spec.width = int(op.attrib.get('width'))
+        if op.attrib.get('s', '1') == '0':
+            spec.signed = False
         return spec
 
     @staticmethod
     def parse_label_operand(_):
         spec = OperandSpec()
         spec.type_ = "LABEL"
         spec.values = []
@@ -300,15 +303,15 @@
     def __init__(self, extensions: List[str], out_file: str) -> None:
         self.extensions = extensions
         self.out_file = out_file
 
     def run(self):
         subprocess.run(
             "wget "
-            "https://github.com/microsoft/sca-fuzzer/releases/download/v1.2/x86_instructions.xml",
+            "https://github.com/microsoft/sca-fuzzer/releases/download/v1.2.4/x86_instructions.xml",
             shell=True,
             check=True)
 
         try:
             transformer = X86Transformer()
             transformer.load_files("x86_instructions.xml")
             transformer.parse_tree(self.extensions)
```

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_config.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_config.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_executor.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_executor.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_fuzzer.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_fuzzer.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_generator.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_generator.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_model.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_model.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/revizor/x86/x86_target_desc.py` & `revizor_fuzzer-1.2.4/revizor/x86/x86_target_desc.py`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/LICENSE` & `revizor_fuzzer-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revizor_fuzzer-1.2.3/README.md` & `revizor_fuzzer-1.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -197,14 +197,35 @@
 
 If something is confusing or you need help in using Revizor, we have a [discussion page](https://github.com/microsoft/sca-fuzzer/discussions).
 
 ## Documentation
 
 For more details, see [the website](https://microsoft.github.io/sca-fuzzer/).
 
+
+## Citing Revizor
+
+To cite this project, you can use the following references:
+
+1. The original paper that introduced the concepts of Model-based Relation Testing, and which describes the main ideas behind Revizor.
+ 
+    Oleksii Oleksenko, Christof Fetzer, Boris Köpf, Mark Silberstein. "[Revizor: Testing Black-box CPUs against Speculation Contracts](https://www.microsoft.com/en-us/research/publication/revizor-testing-black-box-cpus-against-speculation-contracts/)" in Proceedings of the 27th ACM International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS), 2022.
+
+2. The paper that introduced the idea of Leakage Contracts, as well as its theoretical foundations.
+
+    Marco Guarnieri, Boris Köpf, Jan Reineke, and Pepe Vila. "[Hardware-software contracts for secure speculation](https://www.microsoft.com/en-us/research/publication/hardware-software-contracts-for-secure-speculation/)" in Proceedings of the 2021 IEEE Symposium on Security and Privacy (SP), 2021.
+
+3. A more accessible summary of the two papers above, in a journal format.
+
+    Oleksii Oleksenko, Christof Fetzer, Boris Köpf, Mark Silberstein. "Revizor: Testing Black-box CPUs against Speculation Contracts". In IEEE Micro, 2023.
+
+4. The paper that introduced taint-based input generation, speculation filtering, and observation filtering:
+
+    Oleksii Oleksenko, Marco Guarnieri, Boris Köpf, and Mark Silberstein. "[Hide and Seek with Spectres: Efficient discovery of speculative information leaks with random testing](https://www.microsoft.com/en-us/research/publication/hide-and-seek-with-spectres-efficient-discovery-of-speculative-information-leaks-with-random-testing/)" in Proceedings of the 2023 IEEE Symposium on Security and Privacy (SP), 2022.
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Trademarks
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `revizor_fuzzer-1.2.3/pyproject.toml` & `revizor_fuzzer-1.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revizor-fuzzer"
-version = "1.2.3"
+version = "1.2.4"
 description = "A fuzzer to search for microarchitectural leaks in CPUs"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
@@ -40,7 +40,10 @@
   "src/tests/",
   "src/x86/executor/",
   "src/x86/tests/",
 ]
 
 [project.scripts]
 rvzr = "revizor.cli:main"
+
+[tool.hatch.build.targets.wheel]
+packages = ["revizor"]
```

### Comparing `revizor_fuzzer-1.2.3/PKG-INFO` & `revizor_fuzzer-1.2.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: revizor-fuzzer
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fuzzer to search for microarchitectural leaks in CPUs
 Project-URL: Homepage, https://microsoft.github.io/sca-fuzzer/
 Project-URL: Source code, https://github.com/microsoft/sca-fuzzer
 Project-URL: Bug Tracker, https://github.com/microsoft/sca-fuzzer/issues
 Project-URL: Changelog, https://github.com/microsoft/sca-fuzzer/releases
 Maintainer: Oleksii Oleksenko
 License-File: AUTHORS
@@ -220,14 +220,35 @@
 
 If something is confusing or you need help in using Revizor, we have a [discussion page](https://github.com/microsoft/sca-fuzzer/discussions).
 
 ## Documentation
 
 For more details, see [the website](https://microsoft.github.io/sca-fuzzer/).
 
+
+## Citing Revizor
+
+To cite this project, you can use the following references:
+
+1. The original paper that introduced the concepts of Model-based Relation Testing, and which describes the main ideas behind Revizor.
+ 
+    Oleksii Oleksenko, Christof Fetzer, Boris Köpf, Mark Silberstein. "[Revizor: Testing Black-box CPUs against Speculation Contracts](https://www.microsoft.com/en-us/research/publication/revizor-testing-black-box-cpus-against-speculation-contracts/)" in Proceedings of the 27th ACM International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS), 2022.
+
+2. The paper that introduced the idea of Leakage Contracts, as well as its theoretical foundations.
+
+    Marco Guarnieri, Boris Köpf, Jan Reineke, and Pepe Vila. "[Hardware-software contracts for secure speculation](https://www.microsoft.com/en-us/research/publication/hardware-software-contracts-for-secure-speculation/)" in Proceedings of the 2021 IEEE Symposium on Security and Privacy (SP), 2021.
+
+3. A more accessible summary of the two papers above, in a journal format.
+
+    Oleksii Oleksenko, Christof Fetzer, Boris Köpf, Mark Silberstein. "Revizor: Testing Black-box CPUs against Speculation Contracts". In IEEE Micro, 2023.
+
+4. The paper that introduced taint-based input generation, speculation filtering, and observation filtering:
+
+    Oleksii Oleksenko, Marco Guarnieri, Boris Köpf, and Mark Silberstein. "[Hide and Seek with Spectres: Efficient discovery of speculative information leaks with random testing](https://www.microsoft.com/en-us/research/publication/hide-and-seek-with-spectres-efficient-discovery-of-speculative-information-leaks-with-random-testing/)" in Proceedings of the 2023 IEEE Symposium on Security and Privacy (SP), 2022.
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Trademarks
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

