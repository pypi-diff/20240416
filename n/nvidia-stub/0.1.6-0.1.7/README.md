# Comparing `tmp/nvidia_stub-0.1.6-py3-none-any.whl.zip` & `tmp/nvidia_stub-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 66401 bytes, number of entries: 30
+Zip file size: 66369 bytes, number of entries: 30
 -rw-r--r--  2.0 unx      739 b- defN 20-Feb-02 00:00 nvidia_stub/ERROR.txt
 -rwxr-xr-x  2.0 unx      701 b- defN 20-Feb-02 00:00 nvidia_stub/__about__.py
 -rwxr-xr-x  2.0 unx      679 b- defN 20-Feb-02 00:00 nvidia_stub/__init__.py
 -rwxr-xr-x  2.0 unx     1598 b- defN 20-Feb-02 00:00 nvidia_stub/buildapi.py
 -rw-r--r--  2.0 unx      890 b- defN 20-Feb-02 00:00 nvidia_stub/common.py
 -rw-r--r--  2.0 unx     2758 b- defN 20-Feb-02 00:00 nvidia_stub/error.py
 -rwxr-xr-x  2.0 unx     6269 b- defN 20-Feb-02 00:00 nvidia_stub/sdist.py
--rw-r--r--  2.0 unx     5540 b- defN 20-Feb-02 00:00 nvidia_stub/wheel.py
+-rw-r--r--  2.0 unx     5482 b- defN 20-Feb-02 00:00 nvidia_stub/wheel.py
 -rw-r--r--  2.0 unx      407 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/README.md
 -rw-r--r--  2.0 unx      681 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/__init__.py
 -rw-r--r--  2.0 unx    11758 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/LICENSE
 -rw-r--r--  2.0 unx      496 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/__init__.py
 -rw-r--r--  2.0 unx     3266 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/_elffile.py
 -rw-r--r--  2.0 unx     9526 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/_manylinux.py
 -rw-r--r--  2.0 unx     2676 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/_musllinux.py
@@ -21,12 +21,12 @@
 -rw-r--r--  2.0 unx    32750 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/metadata.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/py.typed
 -rw-r--r--  2.0 unx     2952 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/requirements.py
 -rw-r--r--  2.0 unx    39206 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/specifiers.py
 -rw-r--r--  2.0 unx    18355 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/tags.py
 -rw-r--r--  2.0 unx     5268 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/utils.py
 -rw-r--r--  2.0 unx    16236 b- defN 20-Feb-02 00:00 nvidia_stub/_vendor/packaging/version.py
-?rw-r--r--  2.0 unx      701 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.6.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx    10457 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.6.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     2683 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.6.dist-info/RECORD
-30 files, 201992 bytes uncompressed, 62033 bytes compressed:  69.3%
+?rw-r--r--  2.0 unx      701 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx    10457 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     2683 b- defN 20-Feb-02 00:00 nvidia_stub-0.1.7.dist-info/RECORD
+30 files, 201934 bytes uncompressed, 62001 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: nvidia_stub/_vendor/packaging/utils.py
 Comment: 
 
 Filename: nvidia_stub/_vendor/packaging/version.py
 Comment: 
 
-Filename: nvidia_stub-0.1.6.dist-info/METADATA
+Filename: nvidia_stub-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_stub-0.1.6.dist-info/WHEEL
+Filename: nvidia_stub-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_stub-0.1.6.dist-info/licenses/LICENSE
+Filename: nvidia_stub-0.1.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: nvidia_stub-0.1.6.dist-info/RECORD
+Filename: nvidia_stub-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia_stub/__about__.py

```diff
@@ -8,8 +8,8 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

## nvidia_stub/wheel.py

```diff
@@ -60,17 +60,16 @@
             if i == num_retries:
                 raise
         time.sleep(1.2**i)
 
 
 def is_compatible_tag(tag, this_interp_tag, system_tags):
     if tag.abi == "none":
-        # Only install platform agnostic wheels that don't declare an ABI
-        if tag.interpreter in ["any", "py3", this_interp_tag]:
-            return True
+        if tag.interpreter in ["py3", this_interp_tag]:
+            return tag.platform in system_tags
         else:
             return False
     elif tag.abi == this_interp_tag:
         # If the ABI is for this interpreter, the interpreter tag must be this interpreters
         if tag.interpreter != this_interp_tag:
             return False
     elif tag.abi == "abi3":
```

## Comparing `nvidia_stub-0.1.6.dist-info/METADATA` & `nvidia_stub-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nvidia-stub
-Version: 0.1.6
+Version: 0.1.7
 Summary: NVIDIA stub package build backend
 Author-email: Ethan Smith <etsmith@nvidia.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `nvidia_stub-0.1.6.dist-info/licenses/LICENSE` & `nvidia_stub-0.1.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `nvidia_stub-0.1.6.dist-info/RECORD` & `nvidia_stub-0.1.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 nvidia_stub/ERROR.txt,sha256=4VHd5PHhzFY6ya4MP1aZfaJcSB1wm2lVNYEAQl_LhIs,739
-nvidia_stub/__about__.py,sha256=H77ImgNBWG7KpKx380of10zuFczyGgkllFfwq-t4v2M,701
+nvidia_stub/__about__.py,sha256=OWpwRra_R-KTzzwgakXuWSajO7JkEblE7KNCbUkBTcc,701
 nvidia_stub/__init__.py,sha256=3QMzksa2HTcOPG6-2RTwrhBfDYG6S4d4WfamF9D-2tY,679
 nvidia_stub/buildapi.py,sha256=URQ9VNKLoMSlUiVFIH8VrlvE3QX8XNat-mxsKV9D85U,1598
 nvidia_stub/common.py,sha256=TWUoYqHsD2rHgv_gmwCkRxgoOguwqrR7N2glUSMjvPY,890
 nvidia_stub/error.py,sha256=w1hp4DzyhUX8_mkjsRx1oQ_kjY_p5OjZUUpgwkvecHw,2758
 nvidia_stub/sdist.py,sha256=rGa3DKXfbnZvvQsHqu6jZUvzih9rQRgtWbgsXzk2xRA,6269
-nvidia_stub/wheel.py,sha256=u4fpM3y2Gok-cf9Bo18GsjbscCVTfWd5TvChjXtu8NY,5540
+nvidia_stub/wheel.py,sha256=AWkEfChAHH84Ksc3SPoVW1mFIFvbrKp0GxHl1a_oxb4,5482
 nvidia_stub/_vendor/README.md,sha256=GoQShkg93cDCQ_rKph50sIrEpNumklX69C6KEIuBPw8,407
 nvidia_stub/_vendor/__init__.py,sha256=hVTZxDwMNMxOuyukwh99PSywvfi7yK9Y2y8u--bi2HM,681
 nvidia_stub/_vendor/packaging/LICENSE,sha256=l6_dQpYMiqBcWKkYZ6lXfd0oonjPVbMDkVIm-e5fon0,11758
 nvidia_stub/_vendor/packaging/__init__.py,sha256=EhCMuCSz60IgQJ93b_4wJyAoHpU9J-uddG4QaMT0Pu4,496
 nvidia_stub/_vendor/packaging/_elffile.py,sha256=hbmK8OD6Z7fY6hwinHEUcD1by7czkGiNYu7ShnFEk2k,3266
 nvidia_stub/_vendor/packaging/_manylinux.py,sha256=Rq6ppXAxH8XFtNf6tC-B-1SKuvCODPBvcCoSulMtbtk,9526
 nvidia_stub/_vendor/packaging/_musllinux.py,sha256=kgmBGLFybpy8609-KTvzmt2zChCPWYvhp5BWP4JX7dE,2676
@@ -20,11 +20,11 @@
 nvidia_stub/_vendor/packaging/metadata.py,sha256=ToxjINOmSn8mbEeXRSVNMidEJsPUYHEYFnnN4MaqvH0,32750
 nvidia_stub/_vendor/packaging/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia_stub/_vendor/packaging/requirements.py,sha256=wswG4mXHSgE9w4NjNnlSvgLGo6yYvfHVEFnWhuEmXxg,2952
 nvidia_stub/_vendor/packaging/specifiers.py,sha256=ZOpqL_w_Kj6ZF_OWdliQUzhEyHlDbi6989kr-sF5GHs,39206
 nvidia_stub/_vendor/packaging/tags.py,sha256=pkG6gQ28RlhS09VzymVhVpGrWF5doHXfK1VxG9cdhoY,18355
 nvidia_stub/_vendor/packaging/utils.py,sha256=XgdmP3yx9-wQEFjO7OvMj9RjEf5JlR5HFFR69v7SQ9E,5268
 nvidia_stub/_vendor/packaging/version.py,sha256=XjRBLNK17UMDgLeP8UHnqwiY3TdSi03xFQURtec211A,16236
-nvidia_stub-0.1.6.dist-info/METADATA,sha256=yYZEoH7KAqffUdaewc5qvN54eImqipIQUW31-yWqcRc,701
-nvidia_stub-0.1.6.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
-nvidia_stub-0.1.6.dist-info/licenses/LICENSE,sha256=3dE0gNVm97tFh-wCShhDUaZP6w7J5p90s94W60UYcXo,10457
-nvidia_stub-0.1.6.dist-info/RECORD,,
+nvidia_stub-0.1.7.dist-info/METADATA,sha256=FXaaoq2ldMu2SsipTiyDOwHAwsNpI4me8yWX2dVtR7A,701
+nvidia_stub-0.1.7.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
+nvidia_stub-0.1.7.dist-info/licenses/LICENSE,sha256=3dE0gNVm97tFh-wCShhDUaZP6w7J5p90s94W60UYcXo,10457
+nvidia_stub-0.1.7.dist-info/RECORD,,
```

