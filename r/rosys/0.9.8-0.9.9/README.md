# Comparing `tmp/rosys-0.9.8.tar.gz` & `tmp/rosys-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosys-0.9.8.tar", max compression
+gzip compressed data, was "rosys-0.9.9.tar", max compression
```

## Comparing `rosys-0.9.8.tar` & `rosys-0.9.9.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     1072 2023-12-27 10:19:46.378188 rosys-0.9.8/LICENSE
--rw-r--r--   0        0        0     6602 2023-12-27 10:19:46.378188 rosys-0.9.8/README.md
--rw-r--r--   0        0        0     1775 2023-12-27 10:20:02.074128 rosys-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       28 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/.syncignore
--rw-r--r--   0        0        0      457 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/__init__.py
--rw-r--r--   0        0        0      581 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/__init__.py
--rw-r--r--   0        0        0    86820 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/assets/RobotoMono-Medium.ttf
--rw-r--r--   0        0        0     1833 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/asyncio_warnings.py
--rw-r--r--   0        0        0      753 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/kpi_buckets.py
--rw-r--r--   0        0        0     2085 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/kpi_logger.py
--rw-r--r--   0        0        0     4549 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/kpi_page_.py
--rw-r--r--   0        0        0        0 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/__init__.py
--rw-r--r--   0        0        0     3237 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/asyncio_monitor.py
--rw-r--r--   0        0        0     1728 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/asyncio_page.py
--rw-r--r--   0        0        0     1970 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/network_monitor.py
--rw-r--r--   0        0        0     3103 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/objgraph_page.py
--rw-r--r--   0        0        0      703 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/legacy/pyloot_page.py
--rw-r--r--   0        0        0     2547 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/memory.py
--rw-r--r--   0        0        0     1659 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/profile_button_.py
--rw-r--r--   0        0        0     1064 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/profiling.py
--rw-r--r--   0        0        0     6656 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/timelapse_recorder.py
--rw-r--r--   0        0        0      828 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/track.py
--rw-r--r--   0        0        0     1035 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/analysis/videos_page_.py
--rw-r--r--   0        0        0      269 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/__init__.py
--rw-r--r--   0        0        0     5132 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/app_controls_.py
--rw-r--r--   0        0        0     2807 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/automation.py
--rw-r--r--   0        0        0     1475 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/automation_controls_.py
--rw-r--r--   0        0        0     5985 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/automator.py
--rw-r--r--   0        0        0     1546 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/parallelize.py
--rw-r--r--   0        0        0     9883 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/automation/schedule.py
--rw-r--r--   0        0        0      464 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/config.py
--rw-r--r--   0        0        0      422 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/__init__.py
--rw-r--r--   0        0        0      194 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/drivable.py
--rw-r--r--   0        0        0     8696 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/driver.py
--rw-r--r--   0        0        0     1979 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/driver_object.py
--rw-r--r--   0        0        0      596 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/joystick_.py
--rw-r--r--   0        0        0     2230 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/keyboard_control_.py
--rw-r--r--   0        0        0     3759 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/odometer.py
--rw-r--r--   0        0        0      169 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/path_segment.py
--rw-r--r--   0        0        0     1821 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/robot_object_.py
--rw-r--r--   0        0        0     3060 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/driving/steerer.py
--rw-r--r--   0        0        0     3015 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/event.py
--rw-r--r--   0        0        0      324 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/__init__.py
--rw-r--r--   0        0        0     1193 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/line.py
--rw-r--r--   0        0        0     1649 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/line_segment.py
--rw-r--r--   0        0        0     2223 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/point.py
--rw-r--r--   0        0        0      915 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/point3d.py
--rw-r--r--   0        0        0      503 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/polygon.py
--rw-r--r--   0        0        0     4377 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/pose.py
--rw-r--r--   0        0        0      344 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/prism.py
--rw-r--r--   0        0        0      658 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/rectangle.py
--rw-r--r--   0        0        0     1785 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/rotation.py
--rw-r--r--   0        0        0    10572 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/spline.py
--rw-r--r--   0        0        0      142 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/geometry/velocity.py
--rw-r--r--   0        0        0      687 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/__init__.py
--rw-r--r--   0        0        0     1324 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/battery_control.py
--rw-r--r--   0        0        0      341 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/bluetooth.py
--rw-r--r--   0        0        0     4628 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/bms.py
--rw-r--r--   0        0        0     3115 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/bms_message.py
--rw-r--r--   0        0        0      770 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/bms_state.py
--rw-r--r--   0        0        0     2400 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/bumper.py
--rw-r--r--   0        0        0      657 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/can.py
--rw-r--r--   0        0        0      143 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/communication/__init__.py
--rw-r--r--   0        0        0      844 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/communication/communication.py
--rw-r--r--   0        0        0     4205 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/communication/serial_communication.py
--rw-r--r--   0        0        0     1452 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/communication/web_communication.py
--rw-r--r--   0        0        0     2362 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/estop.py
--rw-r--r--   0        0        0      637 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/expander.py
--rwxr-xr-x   0        0        0     1185 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/hardware_proxy.py
--rw-r--r--   0        0        0      265 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/imu.py
--rw-r--r--   0        0        0     4903 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/lizard_firmware.py
--rw-r--r--   0        0        0      877 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/module.py
--rw-r--r--   0        0        0     2646 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/robot.py
--rw-r--r--   0        0        0     8275 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/robot_brain.py
--rw-r--r--   0        0        0      607 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/serial.py
--rw-r--r--   0        0        0     4113 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/hardware/wheels.py
--rw-r--r--   0        0        0     3820 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/helpers.py
--rw-r--r--   0        0        0      330 2023-12-27 10:19:46.394187 rosys-0.9.8/rosys/pathplanning/__init__.py
--rw-r--r--   0        0        0     1372 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/area.py
--rw-r--r--   0        0        0     7283 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/area_manipulation.py
--rw-r--r--   0        0        0     2497 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/area_object_.py
--rw-r--r--   0        0        0     1372 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/binary_renderer.py
--rwxr-xr-x   0        0        0     1096 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/binary_renderer_demo.py
--rw-r--r--   0        0        0    14725 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/delaunay_planner.py
--rw-r--r--   0        0        0      220 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/delaunay_pose_group.py
--rw-r--r--   0        0        0     2831 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220714-1.py
--rw-r--r--   0        0        0     2943 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220714-2-A.py
--rw-r--r--   0        0        0     2939 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220714-2-B.py
--rw-r--r--   0        0        0     2940 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220714-3.py
--rw-r--r--   0        0        0     3196 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220725-1.py
--rw-r--r--   0        0        0    38753 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220825-1.py
--rw-r--r--   0        0        0    16920 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220916-1.py
--rw-r--r--   0        0        0     3907 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20220921-1.py
--rw-r--r--   0        0        0     4217 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20221121-1.py
--rw-r--r--   0        0        0     4220 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20221203-1.py
--rw-r--r--   0        0        0    32139 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20230120-1.py
--rw-r--r--   0        0        0     3876 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20230605-1.py
--rw-r--r--   0        0        0     8405 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20231031-1.py
--rw-r--r--   0        0        0    36608 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/demos/20231102-1.py
--rw-r--r--   0        0        0     2948 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/distance_map.py
--rwxr-xr-x   0        0        0     1804 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/distance_map_demo.py
--rw-r--r--   0        0        0     1843 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/experiments.py
--rwxr-xr-x   0        0        0      476 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/experiments_demo.py
--rw-r--r--   0        0        0     1935 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/fast_spline.py
--rw-r--r--   0        0        0     2678 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/grid.py
--rwxr-xr-x   0        0        0      515 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/grid_demo.py
--rw-r--r--   0        0        0      156 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/obstacle.py
--rw-r--r--   0        0        0     4487 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/obstacle_map.py
--rwxr-xr-x   0        0        0     1256 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/obstacle_map_demo.py
--rw-r--r--   0        0        0      832 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/obstacle_object_.py
--rw-r--r--   0        0        0      937 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/path_object_.py
--rw-r--r--   0        0        0     5304 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/path_planner.py
--rwxr-xr-x   0        0        0     3066 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/planner_demo.py
--rw-r--r--   0        0        0     3230 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/planner_process.py
--rw-r--r--   0        0        0     1962 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/plot_tools.py
--rwxr-xr-x   0        0        0     1240 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/plot_tools_demo.py
--rw-r--r--   0        0        0     1081 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/robot_renderer.py
--rwxr-xr-x   0        0        0      625 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/robot_renderer_demo.py
--rw-r--r--   0        0        0     2759 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/steps.py
--rwxr-xr-x   0        0        0     1750 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/pathplanning/steps_demo.py
--rw-r--r--   0        0        0      580 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/persistence/__init__.py
--rw-r--r--   0        0        0     1411 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/persistence/converters.py
--rw-r--r--   0        0        0      795 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/persistence/persistent_module.py
--rw-r--r--   0        0        0     1529 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/persistence/registry.py
--rw-r--r--   0        0        0     1302 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/persistence/ui.py
--rw-r--r--   0        0        0     8029 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/rosys.py
--rw-r--r--   0        0        0     5289 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/run.py
--rw-r--r--   0        0        0      636 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/simulation_ui.py
--rw-r--r--   0        0        0       52 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/system/__init__.py
--rw-r--r--   0        0        0     2107 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/system/wifi_button_.py
--rw-r--r--   0        0        0      234 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/test/__init__.py
--rw-r--r--   0        0        0     4638 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/test/helpers.py
--rw-r--r--   0        0        0     2089 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/test/log_configuration.py
--rw-r--r--   0        0        0      807 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/__init__.py
--rw-r--r--   0        0        0     5551 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/calibration.py
--rw-r--r--   0        0        0      293 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera/__init__.py
--rw-r--r--   0        0        0     1427 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera/calibratable_camera.py
--rw-r--r--   0        0        0     3898 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera/camera.py
--rw-r--r--   0        0        0     3005 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera/configurable_camera.py
--rw-r--r--   0        0        0     1544 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera/transformable_camera.py
--rw-r--r--   0        0        0     4852 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera_objects_.py
--rw-r--r--   0        0        0     2803 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera_projector.py
--rw-r--r--   0        0        0     2522 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/camera_provider.py
--rw-r--r--   0        0        0     3986 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/detections.py
--rw-r--r--   0        0        0     1398 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/detector.py
--rw-r--r--   0        0        0     7070 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/detector_hardware.py
--rw-r--r--   0        0        0     4649 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/detector_simulation.py
--rw-r--r--   0        0        0     2183 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/image.py
--rw-r--r--   0        0        0     1975 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/image_processing.py
--rw-r--r--   0        0        0      409 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/image_rotation.py
--rw-r--r--   0        0        0     2138 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/image_route.py
--rw-r--r--   0        0        0      639 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/multi_camera_provider.py
--rw-r--r--   0        0        0      148 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/__init__.py
--rw-r--r--   0        0        0     1757 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/arp_scan.py
--rw-r--r--   0        0        0     5339 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/jovision_rtsp_interface.py
--rw-r--r--   0        0        0     4518 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_camera.py
--rw-r--r--   0        0        0     2423 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_camera_provider.py
--rw-r--r--   0        0        0     4618 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_device.py
--rw-r--r--   0        0        0      679 2023-12-27 10:19:46.398187 rosys-0.9.8/rosys/vision/rtsp_camera/vendors.py
--rw-r--r--   0        0        0      178 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/simulated_camera/__init__.py
--rw-r--r--   0        0        0     2508 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/simulated_camera/simulated_camera.py
--rw-r--r--   0        0        0     1969 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/simulated_camera/simulated_camera_provider.py
--rw-r--r--   0        0        0     1373 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/simulated_camera/simulated_device.py
--rw-r--r--   0        0        0     1004 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/uploads.py
--rw-r--r--   0        0        0      142 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/usb_camera/__init__.py
--rw-r--r--   0        0        0     6598 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/usb_camera/usb_camera.py
--rw-r--r--   0        0        0     1753 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/usb_camera/usb_camera_provider.py
--rw-r--r--   0        0        0      804 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/usb_camera/usb_camera_scanner.py
--rw-r--r--   0        0        0     3440 2023-12-27 10:19:46.402187 rosys-0.9.8/rosys/vision/usb_camera/usb_device.py
--rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 rosys-0.9.8/setup.py
--rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 rosys-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-06 05:24:17.729995 rosys-0.9.9/LICENSE
+-rw-r--r--   0        0        0     6602 2024-01-06 05:24:17.729995 rosys-0.9.9/README.md
+-rw-r--r--   0        0        0     1775 2024-01-06 05:24:26.418010 rosys-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/.syncignore
+-rw-r--r--   0        0        0      457 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/__init__.py
+-rw-r--r--   0        0        0      581 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/__init__.py
+-rw-r--r--   0        0        0    86820 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/assets/RobotoMono-Medium.ttf
+-rw-r--r--   0        0        0     1833 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/asyncio_warnings.py
+-rw-r--r--   0        0        0      753 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/kpi_buckets.py
+-rw-r--r--   0        0        0     2085 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/kpi_logger.py
+-rw-r--r--   0        0        0     4549 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/kpi_page_.py
+-rw-r--r--   0        0        0        0 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/legacy/__init__.py
+-rw-r--r--   0        0        0     3237 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/legacy/asyncio_monitor.py
+-rw-r--r--   0        0        0     1728 2024-01-06 05:24:17.745995 rosys-0.9.9/rosys/analysis/legacy/asyncio_page.py
+-rw-r--r--   0        0        0     1970 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/legacy/network_monitor.py
+-rw-r--r--   0        0        0     3103 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/legacy/objgraph_page.py
+-rw-r--r--   0        0        0      703 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/legacy/pyloot_page.py
+-rw-r--r--   0        0        0     2547 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/memory.py
+-rw-r--r--   0        0        0     1659 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/profile_button_.py
+-rw-r--r--   0        0        0     1064 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/profiling.py
+-rw-r--r--   0        0        0     6656 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/timelapse_recorder.py
+-rw-r--r--   0        0        0      828 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/track.py
+-rw-r--r--   0        0        0     1175 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/analysis/videos_page_.py
+-rw-r--r--   0        0        0      269 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/__init__.py
+-rw-r--r--   0        0        0     5132 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/app_controls_.py
+-rw-r--r--   0        0        0     2807 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/automation.py
+-rw-r--r--   0        0        0     1475 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/automation_controls_.py
+-rw-r--r--   0        0        0     5985 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/automator.py
+-rw-r--r--   0        0        0     1546 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/parallelize.py
+-rw-r--r--   0        0        0     9883 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/automation/schedule.py
+-rw-r--r--   0        0        0      464 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/config.py
+-rw-r--r--   0        0        0      422 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/__init__.py
+-rw-r--r--   0        0        0      194 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/drivable.py
+-rw-r--r--   0        0        0     8696 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/driver.py
+-rw-r--r--   0        0        0     1979 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/driver_object.py
+-rw-r--r--   0        0        0      596 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/joystick_.py
+-rw-r--r--   0        0        0     2230 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/keyboard_control_.py
+-rw-r--r--   0        0        0     3759 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/odometer.py
+-rw-r--r--   0        0        0      169 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/path_segment.py
+-rw-r--r--   0        0        0     1821 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/robot_object_.py
+-rw-r--r--   0        0        0     3060 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/driving/steerer.py
+-rw-r--r--   0        0        0     3015 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/event.py
+-rw-r--r--   0        0        0      324 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/__init__.py
+-rw-r--r--   0        0        0     1193 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/line.py
+-rw-r--r--   0        0        0     1649 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/line_segment.py
+-rw-r--r--   0        0        0     2223 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/point.py
+-rw-r--r--   0        0        0      915 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/point3d.py
+-rw-r--r--   0        0        0      503 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/polygon.py
+-rw-r--r--   0        0        0     4377 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/pose.py
+-rw-r--r--   0        0        0      344 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/prism.py
+-rw-r--r--   0        0        0      658 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/rectangle.py
+-rw-r--r--   0        0        0     1785 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/rotation.py
+-rw-r--r--   0        0        0    10572 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/spline.py
+-rw-r--r--   0        0        0      142 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/geometry/velocity.py
+-rw-r--r--   0        0        0      687 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/__init__.py
+-rw-r--r--   0        0        0     1324 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/battery_control.py
+-rw-r--r--   0        0        0      341 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/bluetooth.py
+-rw-r--r--   0        0        0     4628 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/bms.py
+-rw-r--r--   0        0        0     3115 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/bms_message.py
+-rw-r--r--   0        0        0      770 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/bms_state.py
+-rw-r--r--   0        0        0     2400 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/bumper.py
+-rw-r--r--   0        0        0      657 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/can.py
+-rw-r--r--   0        0        0      143 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/communication/__init__.py
+-rw-r--r--   0        0        0      844 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/communication/communication.py
+-rw-r--r--   0        0        0     4205 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/communication/serial_communication.py
+-rw-r--r--   0        0        0     1452 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/communication/web_communication.py
+-rw-r--r--   0        0        0     2362 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/estop.py
+-rw-r--r--   0        0        0      637 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/expander.py
+-rwxr-xr-x   0        0        0     1185 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/hardware_proxy.py
+-rw-r--r--   0        0        0      265 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/imu.py
+-rw-r--r--   0        0        0     4903 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/lizard_firmware.py
+-rw-r--r--   0        0        0      877 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/module.py
+-rw-r--r--   0        0        0     2646 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/robot.py
+-rw-r--r--   0        0        0     8275 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/robot_brain.py
+-rw-r--r--   0        0        0      607 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/serial.py
+-rw-r--r--   0        0        0     4113 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/hardware/wheels.py
+-rw-r--r--   0        0        0     3820 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/helpers.py
+-rw-r--r--   0        0        0      330 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/__init__.py
+-rw-r--r--   0        0        0     1372 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/area.py
+-rw-r--r--   0        0        0     7283 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/area_manipulation.py
+-rw-r--r--   0        0        0     2497 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/area_object_.py
+-rw-r--r--   0        0        0     1372 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/binary_renderer.py
+-rwxr-xr-x   0        0        0     1096 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/binary_renderer_demo.py
+-rw-r--r--   0        0        0    14725 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/delaunay_planner.py
+-rw-r--r--   0        0        0      220 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/delaunay_pose_group.py
+-rw-r--r--   0        0        0     2831 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220714-1.py
+-rw-r--r--   0        0        0     2943 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220714-2-A.py
+-rw-r--r--   0        0        0     2939 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220714-2-B.py
+-rw-r--r--   0        0        0     2940 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220714-3.py
+-rw-r--r--   0        0        0     3196 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220725-1.py
+-rw-r--r--   0        0        0    38753 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220825-1.py
+-rw-r--r--   0        0        0    16920 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220916-1.py
+-rw-r--r--   0        0        0     3907 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20220921-1.py
+-rw-r--r--   0        0        0     4217 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20221121-1.py
+-rw-r--r--   0        0        0     4220 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20221203-1.py
+-rw-r--r--   0        0        0    32139 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20230120-1.py
+-rw-r--r--   0        0        0     3876 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20230605-1.py
+-rw-r--r--   0        0        0     8405 2024-01-06 05:24:17.749995 rosys-0.9.9/rosys/pathplanning/demos/20231031-1.py
+-rw-r--r--   0        0        0    36608 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/demos/20231102-1.py
+-rw-r--r--   0        0        0     2948 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/distance_map.py
+-rwxr-xr-x   0        0        0     1804 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/distance_map_demo.py
+-rw-r--r--   0        0        0     1843 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/experiments.py
+-rwxr-xr-x   0        0        0      476 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/experiments_demo.py
+-rw-r--r--   0        0        0     1935 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/fast_spline.py
+-rw-r--r--   0        0        0     2678 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/grid.py
+-rwxr-xr-x   0        0        0      515 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/grid_demo.py
+-rw-r--r--   0        0        0      156 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/obstacle.py
+-rw-r--r--   0        0        0     4487 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/obstacle_map.py
+-rwxr-xr-x   0        0        0     1256 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/obstacle_map_demo.py
+-rw-r--r--   0        0        0      832 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/obstacle_object_.py
+-rw-r--r--   0        0        0      937 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/path_object_.py
+-rw-r--r--   0        0        0     5304 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/path_planner.py
+-rwxr-xr-x   0        0        0     3066 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/planner_demo.py
+-rw-r--r--   0        0        0     3230 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/planner_process.py
+-rw-r--r--   0        0        0     1962 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/plot_tools.py
+-rwxr-xr-x   0        0        0     1240 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/plot_tools_demo.py
+-rw-r--r--   0        0        0     1081 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/robot_renderer.py
+-rwxr-xr-x   0        0        0      625 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/robot_renderer_demo.py
+-rw-r--r--   0        0        0     2759 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/steps.py
+-rwxr-xr-x   0        0        0     1750 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/pathplanning/steps_demo.py
+-rw-r--r--   0        0        0      580 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/persistence/__init__.py
+-rw-r--r--   0        0        0     1411 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/persistence/converters.py
+-rw-r--r--   0        0        0      795 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/persistence/persistent_module.py
+-rw-r--r--   0        0        0     1529 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/persistence/registry.py
+-rw-r--r--   0        0        0     1302 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/persistence/ui.py
+-rw-r--r--   0        0        0     8029 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/rosys.py
+-rw-r--r--   0        0        0     5289 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/run.py
+-rw-r--r--   0        0        0      636 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/simulation_ui.py
+-rw-r--r--   0        0        0       52 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/system/__init__.py
+-rw-r--r--   0        0        0     2107 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/system/wifi_button_.py
+-rw-r--r--   0        0        0      234 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/test/__init__.py
+-rw-r--r--   0        0        0     4638 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/test/helpers.py
+-rw-r--r--   0        0        0     2089 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/test/log_configuration.py
+-rw-r--r--   0        0        0      807 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/__init__.py
+-rw-r--r--   0        0        0     5551 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/calibration.py
+-rw-r--r--   0        0        0      293 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera/__init__.py
+-rw-r--r--   0        0        0     1427 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera/calibratable_camera.py
+-rw-r--r--   0        0        0     3898 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera/camera.py
+-rw-r--r--   0        0        0     3005 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera/configurable_camera.py
+-rw-r--r--   0        0        0     1544 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera/transformable_camera.py
+-rw-r--r--   0        0        0     4852 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera_objects_.py
+-rw-r--r--   0        0        0     2803 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera_projector.py
+-rw-r--r--   0        0        0     2522 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/camera_provider.py
+-rw-r--r--   0        0        0     3986 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/detections.py
+-rw-r--r--   0        0        0     1398 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/detector.py
+-rw-r--r--   0        0        0     7070 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/detector_hardware.py
+-rw-r--r--   0        0        0     4649 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/detector_simulation.py
+-rw-r--r--   0        0        0     2183 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/image.py
+-rw-r--r--   0        0        0     1975 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/image_processing.py
+-rw-r--r--   0        0        0      409 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/image_rotation.py
+-rw-r--r--   0        0        0     2138 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/image_route.py
+-rw-r--r--   0        0        0      639 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/multi_camera_provider.py
+-rw-r--r--   0        0        0      148 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/__init__.py
+-rw-r--r--   0        0        0     1757 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/arp_scan.py
+-rw-r--r--   0        0        0     5339 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/jovision_rtsp_interface.py
+-rw-r--r--   0        0        0     4518 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_camera.py
+-rw-r--r--   0        0        0     2423 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_camera_provider.py
+-rw-r--r--   0        0        0     4618 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_device.py
+-rw-r--r--   0        0        0      679 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/rtsp_camera/vendors.py
+-rw-r--r--   0        0        0      178 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/simulated_camera/__init__.py
+-rw-r--r--   0        0        0     2508 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/simulated_camera/simulated_camera.py
+-rw-r--r--   0        0        0     1969 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/simulated_camera/simulated_camera_provider.py
+-rw-r--r--   0        0        0     1373 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/simulated_camera/simulated_device.py
+-rw-r--r--   0        0        0     1004 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/uploads.py
+-rw-r--r--   0        0        0      142 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/usb_camera/__init__.py
+-rw-r--r--   0        0        0     6622 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/usb_camera/usb_camera.py
+-rw-r--r--   0        0        0     1753 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/usb_camera/usb_camera_provider.py
+-rw-r--r--   0        0        0      804 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/usb_camera/usb_camera_scanner.py
+-rw-r--r--   0        0        0     3440 2024-01-06 05:24:17.753995 rosys-0.9.9/rosys/vision/usb_camera/usb_device.py
+-rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 rosys-0.9.9/setup.py
+-rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 rosys-0.9.9/PKG-INFO
```

### Comparing `rosys-0.9.8/LICENSE` & `rosys-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/README.md` & `rosys-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/pyproject.toml` & `rosys-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rosys"
-version = "v0.9.8"
+version = "v0.9.9"
 description = "Modular Robot System With Elegant Automation Capabilities"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/rosys"
 keywords = ["robot", "framework", "automation", "control", "steer"]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
-nicegui = ">=1.4.8"
+nicegui = ">=1.4.9"
 asyncio = "^3.4.3"
 retry = "^0.9.2"
 requests = "^2.25.1"
 urllib3 = "^2.0.6" # https://github.com/zauberzeug/rosys/security/dependabot/31
 aiohttp = "^3.9.0" # https://github.com/zauberzeug/rosys/security/dependabot/35
 simplejson = "^3.17.2"
 pyserial = "^3.5"
```

### Comparing `rosys-0.9.8/rosys/analysis/__init__.py` & `rosys-0.9.9/rosys/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/assets/RobotoMono-Medium.ttf` & `rosys-0.9.9/rosys/analysis/assets/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/asyncio_warnings.py` & `rosys-0.9.9/rosys/analysis/asyncio_warnings.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/kpi_buckets.py` & `rosys-0.9.9/rosys/analysis/kpi_buckets.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/kpi_logger.py` & `rosys-0.9.9/rosys/analysis/kpi_logger.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/kpi_page_.py` & `rosys-0.9.9/rosys/analysis/kpi_page_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/legacy/asyncio_monitor.py` & `rosys-0.9.9/rosys/analysis/legacy/asyncio_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/legacy/asyncio_page.py` & `rosys-0.9.9/rosys/analysis/legacy/asyncio_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/legacy/network_monitor.py` & `rosys-0.9.9/rosys/analysis/legacy/network_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/legacy/objgraph_page.py` & `rosys-0.9.9/rosys/analysis/legacy/objgraph_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/legacy/pyloot_page.py` & `rosys-0.9.9/rosys/analysis/legacy/pyloot_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/memory.py` & `rosys-0.9.9/rosys/analysis/memory.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/profile_button_.py` & `rosys-0.9.9/rosys/analysis/profile_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/profiling.py` & `rosys-0.9.9/rosys/analysis/profiling.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/timelapse_recorder.py` & `rosys-0.9.9/rosys/analysis/timelapse_recorder.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/track.py` & `rosys-0.9.9/rosys/analysis/track.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/analysis/videos_page_.py` & `rosys-0.9.9/rosys/analysis/videos_page_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from pathlib import Path
 
 import watchfiles
-from nicegui import background_tasks, ui
+from nicegui import background_tasks, run, ui
 
 VIDEO_FILES = Path('~/.rosys/timelapse/videos').expanduser()
 
 
 class VideosPage:
 
     def __init__(self) -> None:
         @ui.page('/videos', title='Videos')
-        def page():
-
+        async def page():
             @ui.refreshable
-            def videos():
-                for mp4 in sorted(VIDEO_FILES.glob('*.mp4'), reverse=True):
+            async def videos():
+                for mp4 in sorted(await run.io_bound(VIDEO_FILES.glob, '*.mp4'), reverse=True):
                     with ui.row():
                         with ui.card().tight():
-                            ui.video(mp4).classes('w-[800px]')
+                            video = ui.video(mp4).classes('w-[800px]')
+                            src = video._props['src']  # pylint: disable=protected-access
                         with ui.column():
                             ui.button(on_click=lambda mp4=mp4: mp4.unlink()).props('icon=delete flat')
-                            ui.button(on_click=lambda mp4=mp4: ui.download(mp4)).props('icon=download flat')
+                            ui.button(on_click=lambda src=src: ui.download(src)).props('icon=download flat')
 
             async def watch_videos():
                 async for _ in watchfiles.awatch(VIDEO_FILES):
                     videos.refresh()
 
-            videos()
+            await videos()
             background_tasks.create(watch_videos(), name='watch videos files')
```

### Comparing `rosys-0.9.8/rosys/automation/app_controls_.py` & `rosys-0.9.9/rosys/automation/app_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/automation/automation.py` & `rosys-0.9.9/rosys/automation/automation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/automation/automation_controls_.py` & `rosys-0.9.9/rosys/automation/automation_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/automation/automator.py` & `rosys-0.9.9/rosys/automation/automator.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/automation/parallelize.py` & `rosys-0.9.9/rosys/automation/parallelize.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/automation/schedule.py` & `rosys-0.9.9/rosys/automation/schedule.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/driver.py` & `rosys-0.9.9/rosys/driving/driver.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/driver_object.py` & `rosys-0.9.9/rosys/driving/driver_object.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/joystick_.py` & `rosys-0.9.9/rosys/driving/joystick_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/keyboard_control_.py` & `rosys-0.9.9/rosys/driving/keyboard_control_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/odometer.py` & `rosys-0.9.9/rosys/driving/odometer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/robot_object_.py` & `rosys-0.9.9/rosys/driving/robot_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/driving/steerer.py` & `rosys-0.9.9/rosys/driving/steerer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/event.py` & `rosys-0.9.9/rosys/event.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/line.py` & `rosys-0.9.9/rosys/geometry/line.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/line_segment.py` & `rosys-0.9.9/rosys/geometry/line_segment.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/point.py` & `rosys-0.9.9/rosys/geometry/point.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/point3d.py` & `rosys-0.9.9/rosys/geometry/point3d.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/pose.py` & `rosys-0.9.9/rosys/geometry/pose.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/rectangle.py` & `rosys-0.9.9/rosys/geometry/rectangle.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/rotation.py` & `rosys-0.9.9/rosys/geometry/rotation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/geometry/spline.py` & `rosys-0.9.9/rosys/geometry/spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/__init__.py` & `rosys-0.9.9/rosys/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/battery_control.py` & `rosys-0.9.9/rosys/hardware/battery_control.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/bms.py` & `rosys-0.9.9/rosys/hardware/bms.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/bms_message.py` & `rosys-0.9.9/rosys/hardware/bms_message.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/bms_state.py` & `rosys-0.9.9/rosys/hardware/bms_state.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/bumper.py` & `rosys-0.9.9/rosys/hardware/bumper.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/can.py` & `rosys-0.9.9/rosys/hardware/can.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/communication/communication.py` & `rosys-0.9.9/rosys/hardware/communication/communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/communication/serial_communication.py` & `rosys-0.9.9/rosys/hardware/communication/serial_communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/communication/web_communication.py` & `rosys-0.9.9/rosys/hardware/communication/web_communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/estop.py` & `rosys-0.9.9/rosys/hardware/estop.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/expander.py` & `rosys-0.9.9/rosys/hardware/expander.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/hardware_proxy.py` & `rosys-0.9.9/rosys/hardware/hardware_proxy.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/lizard_firmware.py` & `rosys-0.9.9/rosys/hardware/lizard_firmware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/module.py` & `rosys-0.9.9/rosys/hardware/module.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/robot.py` & `rosys-0.9.9/rosys/hardware/robot.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/robot_brain.py` & `rosys-0.9.9/rosys/hardware/robot_brain.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/serial.py` & `rosys-0.9.9/rosys/hardware/serial.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/hardware/wheels.py` & `rosys-0.9.9/rosys/hardware/wheels.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/helpers.py` & `rosys-0.9.9/rosys/helpers.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/area.py` & `rosys-0.9.9/rosys/pathplanning/area.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/area_manipulation.py` & `rosys-0.9.9/rosys/pathplanning/area_manipulation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/area_object_.py` & `rosys-0.9.9/rosys/pathplanning/area_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/binary_renderer.py` & `rosys-0.9.9/rosys/pathplanning/binary_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/binary_renderer_demo.py` & `rosys-0.9.9/rosys/pathplanning/binary_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/delaunay_planner.py` & `rosys-0.9.9/rosys/pathplanning/delaunay_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220714-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220714-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220714-2-A.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220714-2-A.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220714-2-B.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220714-2-B.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220714-3.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220714-3.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220725-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220725-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220825-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220825-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220916-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220916-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20220921-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20220921-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20221121-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20221121-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20221203-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20221203-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20230120-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20230120-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20230605-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20230605-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20231031-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20231031-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/demos/20231102-1.py` & `rosys-0.9.9/rosys/pathplanning/demos/20231102-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/distance_map.py` & `rosys-0.9.9/rosys/pathplanning/distance_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/distance_map_demo.py` & `rosys-0.9.9/rosys/pathplanning/distance_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/experiments.py` & `rosys-0.9.9/rosys/pathplanning/experiments.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/fast_spline.py` & `rosys-0.9.9/rosys/pathplanning/fast_spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/grid.py` & `rosys-0.9.9/rosys/pathplanning/grid.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/grid_demo.py` & `rosys-0.9.9/rosys/pathplanning/grid_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/obstacle_map.py` & `rosys-0.9.9/rosys/pathplanning/obstacle_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/obstacle_map_demo.py` & `rosys-0.9.9/rosys/pathplanning/obstacle_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/obstacle_object_.py` & `rosys-0.9.9/rosys/pathplanning/obstacle_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/path_object_.py` & `rosys-0.9.9/rosys/pathplanning/path_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/path_planner.py` & `rosys-0.9.9/rosys/pathplanning/path_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/planner_demo.py` & `rosys-0.9.9/rosys/pathplanning/planner_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/planner_process.py` & `rosys-0.9.9/rosys/pathplanning/planner_process.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/plot_tools.py` & `rosys-0.9.9/rosys/pathplanning/plot_tools.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/plot_tools_demo.py` & `rosys-0.9.9/rosys/pathplanning/plot_tools_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/robot_renderer.py` & `rosys-0.9.9/rosys/pathplanning/robot_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/robot_renderer_demo.py` & `rosys-0.9.9/rosys/pathplanning/robot_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/steps.py` & `rosys-0.9.9/rosys/pathplanning/steps.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/pathplanning/steps_demo.py` & `rosys-0.9.9/rosys/pathplanning/steps_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/persistence/__init__.py` & `rosys-0.9.9/rosys/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/persistence/converters.py` & `rosys-0.9.9/rosys/persistence/converters.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/persistence/persistent_module.py` & `rosys-0.9.9/rosys/persistence/persistent_module.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/persistence/registry.py` & `rosys-0.9.9/rosys/persistence/registry.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/persistence/ui.py` & `rosys-0.9.9/rosys/persistence/ui.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/rosys.py` & `rosys-0.9.9/rosys/rosys.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/run.py` & `rosys-0.9.9/rosys/run.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/simulation_ui.py` & `rosys-0.9.9/rosys/simulation_ui.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/system/wifi_button_.py` & `rosys-0.9.9/rosys/system/wifi_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/test/helpers.py` & `rosys-0.9.9/rosys/test/helpers.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/test/log_configuration.py` & `rosys-0.9.9/rosys/test/log_configuration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/__init__.py` & `rosys-0.9.9/rosys/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/calibration.py` & `rosys-0.9.9/rosys/vision/calibration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera/calibratable_camera.py` & `rosys-0.9.9/rosys/vision/camera/calibratable_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera/camera.py` & `rosys-0.9.9/rosys/vision/camera/camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera/configurable_camera.py` & `rosys-0.9.9/rosys/vision/camera/configurable_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera/transformable_camera.py` & `rosys-0.9.9/rosys/vision/camera/transformable_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera_objects_.py` & `rosys-0.9.9/rosys/vision/camera_objects_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera_projector.py` & `rosys-0.9.9/rosys/vision/camera_projector.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/camera_provider.py` & `rosys-0.9.9/rosys/vision/camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/detections.py` & `rosys-0.9.9/rosys/vision/detections.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/detector.py` & `rosys-0.9.9/rosys/vision/detector.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/detector_hardware.py` & `rosys-0.9.9/rosys/vision/detector_hardware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/detector_simulation.py` & `rosys-0.9.9/rosys/vision/detector_simulation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/image.py` & `rosys-0.9.9/rosys/vision/image.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/image_processing.py` & `rosys-0.9.9/rosys/vision/image_processing.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/image_route.py` & `rosys-0.9.9/rosys/vision/image_route.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/multi_camera_provider.py` & `rosys-0.9.9/rosys/vision/multi_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/arp_scan.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/arp_scan.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/jovision_rtsp_interface.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/jovision_rtsp_interface.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_camera.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_camera_provider.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/rtsp_device.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/rtsp_device.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/rtsp_camera/vendors.py` & `rosys-0.9.9/rosys/vision/rtsp_camera/vendors.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/simulated_camera/simulated_camera.py` & `rosys-0.9.9/rosys/vision/simulated_camera/simulated_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/simulated_camera/simulated_camera_provider.py` & `rosys-0.9.9/rosys/vision/simulated_camera/simulated_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/simulated_camera/simulated_device.py` & `rosys-0.9.9/rosys/vision/simulated_camera/simulated_device.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/uploads.py` & `rosys-0.9.9/rosys/vision/uploads.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/usb_camera/usb_camera.py` & `rosys-0.9.9/rosys/vision/usb_camera/usb_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     async def capture_image(self) -> None:
         if not self.is_connected:
             return None
 
         assert self.device is not None
 
-        capture_success, captured_image = self.device.capture.read()
+        capture_success, captured_image = await rosys.run.io_bound(self.device.capture.read)
         image_is_MJPG = 'MJPG' in self.device.video_formats
 
         if not capture_success:
             await self.disconnect()
             return
 
         if captured_image is None:
```

### Comparing `rosys-0.9.8/rosys/vision/usb_camera/usb_camera_provider.py` & `rosys-0.9.9/rosys/vision/usb_camera/usb_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/usb_camera/usb_camera_scanner.py` & `rosys-0.9.9/rosys/vision/usb_camera/usb_camera_scanner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/rosys/vision/usb_camera/usb_device.py` & `rosys-0.9.9/rosys/vision/usb_camera/usb_device.py`

 * *Files identical despite different names*

### Comparing `rosys-0.9.8/setup.py` & `rosys-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
  'imgsize>=2.1,<3.0',
  'line-profiler>=4.0.3,<5.0.0',
  'matplotlib>=3.7.2,<4.0.0',
  'more-itertools>=8.10.0,<9.0.0',
  'msgpack>=1.0.3,<2.0.0',
  'netifaces>=0.11.0,<0.12.0',
  'networkx>=2.6.2,<3.0.0',
- 'nicegui>=1.4.8',
+ 'nicegui>=1.4.9',
  'numpy>=1.20.1,<2.0.0',
  'objgraph>=3.5.0,<4.0.0',
  'opencv-contrib-python-headless>=4.5.4,<5.0.0',
  'opencv-python>=4.5.5,<5.0.0',
  'psutil>=5.9.0,<6.0.0',
  'pyloot>=0.1.0,<0.2.0',
  'pyserial>=3.5,<4.0',
@@ -60,15 +60,15 @@
  'ujson==5.4.0',
  'urllib3>=2.0.6,<3.0.0',
  'uvloop>=0.17.0,<0.18.0',
  'yappi>=1.4,<2.0']
 
 setup_kwargs = {
     'name': 'rosys',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Modular Robot System With Elegant Automation Capabilities',
     'long_description': '# RoSys - The Robot System\n\nRoSys provides an easy-to-use robot system.\nIts purpose is similar to [ROS](https://www.ros.org/).\nBut RoSys is fully based on modern web technologies and focusses on mobile robotics.\n\nThe full documentation is available at [rosys.io](https://rosys.io/).\n\n## Principles\n\n### All Python\n\nPython is great to write business logic.\nComputation-heavy tasks are wrapped in processes, accessed through WebSockets or called via C++ bindings.\nLike you would do in any other Python program.\n\n### Modularity\n\nYou can structure your code as you please.\nRoSys provides its magic without assuming a specific file structure, configuration files or enforced naming.\n\n### Event Loop\n\nThanks to [asyncio](https://docs.python.org/3/library/asyncio.html) you can write your business logic without locks and mutexes.\nThe execution is [parallel but not concurrent](https://realpython.com/python-concurrency/) which makes it easier to read, write and debug.\nIn real-case scenarios this is also much faster than [ROS](https://www.ros.org/).\nIts multiprocessing architecture requires too much inter-process communication.\n\n### Web UI\n\nMost machines need some kind of human interaction.\nRoSys is built from the ground up to make sure your robot can be operated fully off the grid with any web browser.\nThis is done by incorporating [NiceGUI](https://nicegui.io/), a wonderful all-Python UI web framework.\nIt is also possible to proxy the user interface through a gateway for remote operation.\n\n### Simulation\n\nRobot hardware is often slower than your own computer.\nTo rapidly test out new behavior and algorithms, RoSys provides a simulation mode.\nHere, all hardware is mocked and can even be manipulated to test wheel blockages and similar.\n\n### Testing\n\nYou can use [pytest](https://docs.pytest.org/) to write high-level integration tests.\nIt is based on the above-described simulation mode and accelerates the robot\'s time for super fast execution.\n\n## Architecture and Features\n\n### Modules\n\nRoSys modules are just Python modules which encapsulate certain functionality.\nThey can hold their own state, register lifecycle hooks, run methods repeatedly and subscribe to or raise [events](#events).\nModules can depend on other modules which is mostly implemented by passing them into the constructor.\n\n### Lifecycle Hooks and Loops\n\nModules can register functions via `rosys.on_startup` or `rosys.on_shutdown` as well as repeatedly with a given interval with `rosys.on_repeat`.\n\n<!-- prettier-ignore-start -->\n!!! note\n    Note that NiceGUI\'s `app` object also provides methods `app.on_startup` and `app.on_shutdown`, but it is recommended to use RoSys\' counterparts:\n    `rosys.on_startup` ensures the callback is executed _after_ persistent modules have been loaded from storage.\n    If you, e.g., set the `rosys.config.simulation_speed` programmatically via `app.on_startup()` instead of `rosys.on_startup`,\n    the change is overwritten by RoSys\' `persistence.restore()`.\n<!-- prettier-ignore-end -->\n\n### Events\n\nModules can provide events to allow connecting otherwise separated modules of the system.\nFor example, one module might read sensor data and raise an event `NEW_SENSOR_DATA`, without knowing of any consumers.\nAnother module can register on `NEW_SENSOR_DATA` and act accordingly when being called.\n\n### Automations\n\nRoSys provides an `Automator` module for running "automations".\nAutomations are coroutines that can not only be started and stopped, but also paused and resumed, e.g. using `AutomationControls`.\nHave a look at our [Click-and-drive](examples/click-and-drive.md) example.\n\n### Persistence\n\nModules can register backup and restore methods to read and write their state to disk.\n\n### Time\n\nRoSys uses its own time which is accessible through `rosys.time`.\nThis way the time can advance much faster in simulation and tests if no CPU-intensive operation is performed.\nTo delay the execution of a coroutine, you should invoke `await rosys.sleep(seconds: float)`.\nThis creates a delay until the provided amount of _RoSys time_ has elapsed.\n\n### Threading and Multiprocessing\n\nRoSys makes extensive use of [async/await](#async) to achieve parallelism without threading or multiprocessing.\nBut not every piece of code you want to integrate is offering an asyncio interface.\nTherefore RoSys provides two handy wrappers:\n\nIO-bound:\nIf you need to read from an external device or use a non-async HTTP library like [requests](https://requests.readthedocs.io/),\nyou should wrap the code in a function and await it with `await rosys.run.io_bound(...)`.\n\nCPU-bound:\nIf you need to do some heavy computation and want to spawn another process,\nyou should wrap the code in a function and await it with `await rosys.run.cpu_bound(...)`.\n\n### Safety\n\nPython (and Linux) is fast enough for most high-level logic, but has no realtime guarantees.\nSafety-relevant behavior should therefore be put on a suitable microcontroller.\nIt governs the hardware of the robot and must be able to perform safety actions like triggering emergency hold etc.\n\nWe suggest to use an industrial PC with an integrated controller like the [Zauberzeug Robot Brain](https://www.zauberzeug.com/robot-brain.html).\nIt provides a Linux system to run RoSys, offers AI acceleration via NVidia Jetson, two integrated [ESP32](https://www.espressif.com/en/products/socs/esp32) microcontrollers and six I/O sockets with up to 24 GPIOs for digital I/Os, CAN, RS485, SPI, I2C, etc.\nIt also has two hardware ENABLE switches and one which is controllable via software.\n\nTo have flexible configuration for the microcontroller we created another open source project called [Lizard](https://lizard.dev/).\nIt is a domain-specific language interpreted by the microcontroller which enables you to write reactive hardware behavior without recompiling and flashing.\n\n### User Interface\n\nRoSys builds upon the open source project [NiceGUI](https://nicegui.io/) and offers many robot-related UI elements.\nNiceGUI is a high-level UI framework for the web.\nThis means you can write all UI code in Python and the state is automatically reflected in the browser through WebSockets.\nSee any of our [examples](examples/steering.md).\n\nRoSys can also be used with other user interfaces or interaction models if required, for example a completely app-based control through Bluetooth Low Energy with Flutter.\n\n### Notifications\n\nModules can notify the user through `rosys.notify(\'message to the user\')`.\nWhen using NiceGUI, the notifications will show as snackbar messages.\nThe history of notifications is stored in the list `rosys.notifications`.\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zauberzeug/rosys',
```

### Comparing `rosys-0.9.8/PKG-INFO` & `rosys-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosys
-Version: 0.9.8
+Version: 0.9.9
 Summary: Modular Robot System With Elegant Automation Capabilities
 Home-page: https://github.com/zauberzeug/rosys
 License: MIT
 Keywords: robot,framework,automation,control,steer
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.10,<3.12
@@ -24,15 +24,15 @@
 Requires-Dist: imgsize (>=2.1,<3.0)
 Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: more-itertools (>=8.10.0,<9.0.0)
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: networkx (>=2.6.2,<3.0.0)
-Requires-Dist: nicegui (>=1.4.8)
+Requires-Dist: nicegui (>=1.4.9)
 Requires-Dist: numpy (>=1.20.1,<2.0.0)
 Requires-Dist: objgraph (>=3.5.0,<4.0.0)
 Requires-Dist: opencv-contrib-python-headless (>=4.5.4,<5.0.0)
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyloot (>=0.1.0,<0.2.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
```

