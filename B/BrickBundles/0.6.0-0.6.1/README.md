# Comparing `tmp/brickbundles-0.6.0-py3-none-any.whl.zip` & `tmp/brickbundles-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 109995 bytes, number of entries: 278
+Zip file size: 111393 bytes, number of entries: 281
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Actuator.brick
+-rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/CombustionEngine.brick
 -rw-r--r--  2.0 unx      742 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Differential.brick
 -rw-r--r--  2.0 unx     3717 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
--rw-r--r--  2.0 unx      675 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Engine.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Gear.brick
 -rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Shaft.brick
+-rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/CombustionEngineThrottleInput.brick
+-rw-r--r--  2.0 unx      158 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/CombustionEngineTorqueOutput.brick
 -rw-r--r--  2.0 unx      201 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
 -rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick
 -rw-r--r--  2.0 unx      168 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick
 -rw-r--r--  2.0 unx      171 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterTurbineTorqueOutput.brick
 -rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
 -rw-r--r--  2.0 unx     1193 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick
 -rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueMotor.brick
@@ -62,15 +64,15 @@
 -rw-r--r--  2.0 unx      861 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/Slack/DefaultSlack.brick
 -rw-r--r--  2.0 unx      834 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/Model.brick
 -rw-r--r--  2.0 unx      419 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/PatchElasticity.brick
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/PointwiseElasticity.brick
 -rw-r--r--  2.0 unx      403 b- defN 80-Jan-01 00:00 brickbundles/Physics/KinematicLock.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/BoolInputSignal.brick
 -rw-r--r--  2.0 unx      495 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Input.brick
--rw-r--r--  2.0 unx      265 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/InputOutputType.brick
+-rw-r--r--  2.0 unx      291 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/InputOutputType.brick
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/InputSignal.brick
 -rw-r--r--  2.0 unx      278 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Output.brick
 -rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/OutputSignal.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/RealInputSignal.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/RealOutputSignal.brick
 -rw-r--r--  2.0 unx     1489 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Value.brick
 -rw-r--r--  2.0 unx     1714 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/ValueOutputSignal.brick
@@ -172,14 +174,15 @@
 -rw-r--r--  2.0 unx      818 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/SurfaceContact/PointwiseElasticityDryFrictionModel.brick
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/TorqueMotor.brick
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/TorsionSpring.brick
 -rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/VelocityMotor.brick
 -rw-r--r--  2.0 unx      557 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/RelativeTransform.brick
 -rw-r--r--  2.0 unx      229 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngleOutput.brick
 -rw-r--r--  2.0 unx      276 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick
+-rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/LinearSpringPositionInput.brick
 -rw-r--r--  2.0 unx      290 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick
 -rw-r--r--  2.0 unx      281 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick
 -rw-r--r--  2.0 unx      297 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick
 -rw-r--r--  2.0 unx      280 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick
 -rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick
 -rw-r--r--  2.0 unx      175 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick
 -rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick
@@ -270,11 +273,11 @@
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.6.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    30893 b- defN 16-Jan-01 00:00 brickbundles-0.6.0.dist-info/RECORD
-278 files, 132570 bytes uncompressed, 58007 bytes compressed:  56.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.6.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    31267 b- defN 16-Jan-01 00:00 brickbundles-0.6.1.dist-info/RECORD
+281 files, 134185 bytes uncompressed, 58767 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: brickbundles/DriveTrain/Actuator.brick
 Comment: 
 
-Filename: brickbundles/DriveTrain/Differential.brick
+Filename: brickbundles/DriveTrain/CombustionEngine.brick
 Comment: 
 
-Filename: brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
+Filename: brickbundles/DriveTrain/Differential.brick
 Comment: 
 
-Filename: brickbundles/DriveTrain/Engine.brick
+Filename: brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Gear.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/HingeActuator.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/PrismaticActuator.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Shaft.brick
 Comment: 
 
+Filename: brickbundles/DriveTrain/Signals/CombustionEngineThrottleInput.brick
+Comment: 
+
+Filename: brickbundles/DriveTrain/Signals/CombustionEngineTorqueOutput.brick
+Comment: 
+
 Filename: brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick
@@ -525,14 +531,17 @@
 
 Filename: brickbundles/Physics3D/Signals/HingeAngleOutput.brick
 Comment: 
 
 Filename: brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick
 Comment: 
 
+Filename: brickbundles/Physics3D/Signals/LinearSpringPositionInput.brick
+Comment: 
+
 Filename: brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick
 Comment: 
 
 Filename: brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick
 Comment: 
 
 Filename: brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick
@@ -819,17 +828,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.6.0.dist-info/METADATA
+Filename: brickbundles-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.6.0.dist-info/WHEEL
+Filename: brickbundles-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.6.0.dist-info/RECORD
+Filename: brickbundles-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## brickbundles/Physics/Signals/InputOutputType.brick

```diff
@@ -6,7 +6,8 @@
     Velocity1D is Int: 4
     Velocity3D is Int: 5
     Angle is Int: 6
     AngularVelocity is Int: 7
     Torque is Int: 8
     ControlEvent is Int: 9
     Composite is Int: 10
+    Percentage is Int: 11
```

## Comparing `brickbundles-0.6.0.dist-info/METADATA` & `brickbundles-0.6.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.6.0
+Version: 0.6.1
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.6.0.dist-info/RECORD` & `brickbundles-0.6.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 brickbundles/DriveTrain/Actuator.brick,sha256=x2MlOtidmaIG8Q0FWMu5piL5R9OQMOmD7VIMC9Z3CNM,106
+brickbundles/DriveTrain/CombustionEngine.brick,sha256=M7lNuwyM6azOPVvsnGfzMKesMeux_Sc6-BykGbygGcE,1363
 brickbundles/DriveTrain/Differential.brick,sha256=0wcO8TMm85pxdDeQfNCq75BO7V85jpcYyFdfiCPyB5A,742
 brickbundles/DriveTrain/EmpiricalTorqueConverter.brick,sha256=Dsm0NY3fK1ivflaFViEHI72oQR0GaUAhSb9om9WydYE,3717
-brickbundles/DriveTrain/Engine.brick,sha256=Is3sdxaZfoGcV5D45wSgSN0puv_6cIV1VUUkyt0HSTU,675
 brickbundles/DriveTrain/Gear.brick,sha256=zlJtK6Ii-t08ZXLTZ38lGZlp3_qi8C-8GN5cwTfrbu8,133
 brickbundles/DriveTrain/HingeActuator.brick,sha256=8-8on4lblbEYqyggeL1oJaS9j69zCEAPTEy2WRHuX-o,77
 brickbundles/DriveTrain/PrismaticActuator.brick,sha256=V6w4GIamptmkQDK97VMN2tlMznv1Bmr6iQAw8ckzqyg,246
 brickbundles/DriveTrain/Shaft.brick,sha256=5IwBB9q-73xngtKf3cLJt09lD-QoelUQYZ2miMzFZdw,133
+brickbundles/DriveTrain/Signals/CombustionEngineThrottleInput.brick,sha256=v3U655wGdUSOtrOtOE0-MyRvhtbF8VrGelZrsIGgqh0,162
+brickbundles/DriveTrain/Signals/CombustionEngineTorqueOutput.brick,sha256=4tv7DsjG1_pCht0aYXrXoGAf9HVienILwqy0TzQ7Nfk,158
 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick,sha256=Asi_heEYQ5C7aS3a4KUSyM6VxPBhnBZ0Etfm34PrhhU,201
 brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick,sha256=42E3R72GzNBxdazIgAEojdt1fYlVjATD6bTtHVY0UCY,164
 brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick,sha256=t86UmbtYuJBfqoPpR2Qe3a9zKhfrc9nGRSr2SgSWPro,168
 brickbundles/DriveTrain/Signals/TorqueConverterTurbineTorqueOutput.brick,sha256=JHOvw6eYe0lGO7rx5DanAX1W1KnLjUo3xbz0NAHYtfg,171
 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick,sha256=cUOqFfihVtsq2ZSLq_bDKb6Nl0BOI9zUknnhnFV5SR8,128
 brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick,sha256=rDsDLx-93miXe4vGLukv7zMU9YGlZywUDk73oAGQ34Q,1193
 brickbundles/DriveTrain/TorqueMotor.brick,sha256=eUs07jvCdqwdJiUdiXDmANVAnW1kYNtmwuxuBSUycRM,53
@@ -61,15 +63,15 @@
 brickbundles/Physics/Interactions/Slack/DefaultSlack.brick,sha256=DbTXr9tyv-mtDQ7gwI8mjUktytXoi6WkrzOz2I0tlko,861
 brickbundles/Physics/Interactions/SurfaceContact/Model.brick,sha256=u4eFMWzRQFZJSL23quh-JvTuU22SqOh_i6e-bEVIkD0,834
 brickbundles/Physics/Interactions/SurfaceContact/PatchElasticity.brick,sha256=nWERqV2F0tJ7OxY22nGdKKFqAdmgbwVbKyhQBcgoAQ0,419
 brickbundles/Physics/Interactions/SurfaceContact/PointwiseElasticity.brick,sha256=NSZcYTfuhSrS0TWO8BfObhvpmamWnU21hjFQJqdM2dI,270
 brickbundles/Physics/KinematicLock.brick,sha256=ZWskoZziAF5YZg6BVaWMvoCiB5WL2HlmyD6ei_AoUzU,403
 brickbundles/Physics/Signals/BoolInputSignal.brick,sha256=yaDDXs5x33shckRfFJEVfz6F2uhilQTQG-S_gsYdUFY,121
 brickbundles/Physics/Signals/Input.brick,sha256=I_9js19aE-ax-hT987QHFRvW9uq7adlSSL1q2BQCi6g,495
-brickbundles/Physics/Signals/InputOutputType.brick,sha256=TmkMsr3gs40w_p4lr4gU8lfRQO30Avu1dxqkWANX9Aw,265
+brickbundles/Physics/Signals/InputOutputType.brick,sha256=5eRFMEz7TXa4Hlq0rwGTPIpKGucjwW0TlykO3HTfqsU,291
 brickbundles/Physics/Signals/InputSignal.brick,sha256=S0msuXlEXdi6ZAFA-PkVF9-pFBpvF2W1DMg6RKp2a3E,33
 brickbundles/Physics/Signals/Output.brick,sha256=V1X3nnm4WAMtvMQ8XC9x2UPqNh4DcmlmHP2_tSrVdZc,278
 brickbundles/Physics/Signals/OutputSignal.brick,sha256=khcE8_joHePCV05IXWzYg_SD909fJE08bp3y5C-95VQ,35
 brickbundles/Physics/Signals/RealInputSignal.brick,sha256=MZkPcwAXloiairjyB_Y2RJBl-zEoYf63bc6DA0xuCnE,121
 brickbundles/Physics/Signals/RealOutputSignal.brick,sha256=--co-OVdG6x2CO1P5tmKPWvppOMxrZB7g-ckuMaZArM,121
 brickbundles/Physics/Signals/Value.brick,sha256=CPlTaz0qAjF83i2vASwJ9g-6201hbYZ9m5a3Kk-F1bw,1489
 brickbundles/Physics/Signals/ValueOutputSignal.brick,sha256=Y8Lav3R498DRhfHyfbph1RMlKc5MGdKnTFJfa-ByOvE,1714
@@ -171,14 +173,15 @@
 brickbundles/Physics3D/Interactions/SurfaceContact/PointwiseElasticityDryFrictionModel.brick,sha256=d_D0Ndchzm3BMB3DbKLw634cQcpiYmNSbkJVHjKoolM,818
 brickbundles/Physics3D/Interactions/TorqueMotor.brick,sha256=282nobtKKN3bunaaDNvwcH0YOfPkJdOgMIcUhZRXE2Y,266
 brickbundles/Physics3D/Interactions/TorsionSpring.brick,sha256=1BkWUdDTZEjQ6j89kdzwmx04nFyooCSOs_JSc7By4xY,63
 brickbundles/Physics3D/Interactions/VelocityMotor.brick,sha256=8VLOArZK2RbC1sD_WrA5XoWxm6Ta_kgM9dWy4ISSEA8,1226
 brickbundles/Physics3D/RelativeTransform.brick,sha256=gnAlq_yEiZnwPlOJO37f0CsqDG7vgMUrfs8j5qlvrLA,557
 brickbundles/Physics3D/Signals/HingeAngleOutput.brick,sha256=m550Ce5IXDzvFKTdDUBWBNm8vToDMmEF6MYZDHWLMRk,229
 brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick,sha256=4Ntn2lFfRJcg1_RLcZQElSBdpVIICslr-z4ht36WdeQ,276
+brickbundles/Physics3D/Signals/LinearSpringPositionInput.brick,sha256=6dYgz6RiWRszhQBVfY9NRqZM6G0B4YJFAci9ZmmZOKU,207
 brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick,sha256=Nbe4DmMi7RqEGHW-Bbb0Bvbl5N7LtU9VKnV-LdtIrTs,290
 brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick,sha256=nlATzEPWAoF8VwRXWZY6wLo3jrUttliWLdHA_yNIANY,281
 brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick,sha256=shVe_RZ5BLu4leqOxRAtFmIkJpA0e1RNNXszU5VW4KY,297
 brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick,sha256=mLGtyWb1x65XcXtvBycSd--t2ssmwSBiw8wTWGwhGQ4,280
 brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick,sha256=VTt0g1KwBEpnQNK3aoSRgfiGt10SgyoPnX_PLo9aaOs,289
 brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick,sha256=178qyynryma8abwimrMIj1BxFrcexR4LxsVywhb6umQ,175
 brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick,sha256=aObNKOvwVnGIkTnS9M5qmnpkeK1lcbeAfGVM9eEmtXQ,316
@@ -269,10 +272,10 @@
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.6.0.dist-info/METADATA,sha256=xF_W6UX1VA9rt5cTmb9Vcp5bzxKlsL6EjbuxF1s_dsQ,1066
-brickbundles-0.6.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.6.0.dist-info/RECORD,,
+brickbundles-0.6.1.dist-info/METADATA,sha256=_1giVXAt-N2bol52Mjw0eQcdAc4HPQ-YiAZ6gjgDl-o,1066
+brickbundles-0.6.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.6.1.dist-info/RECORD,,
```

