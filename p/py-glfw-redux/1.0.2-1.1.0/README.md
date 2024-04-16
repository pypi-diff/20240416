# Comparing `tmp/py-glfw-redux-1.0.2.tar.gz` & `tmp/py_glfw_redux-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-glfw-redux-1.0.2.tar", last modified: Tue Mar 19 21:54:39 2024, max compression
+gzip compressed data, was "py_glfw_redux-1.1.0.tar", last modified: Tue Apr 16 00:25:33 2024, max compression
```

## Comparing `py-glfw-redux-1.0.2.tar` & `py_glfw_redux-1.1.0.tar`

### file list

```diff
@@ -1,502 +1,234 @@
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1153 2024-03-18 23:42:02.000000 py-glfw-redux-1.0.2/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1070 2024-03-18 16:31:38.000000 py-glfw-redux-1.0.2/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      103 2024-03-19 21:54:29.000000 py-glfw-redux-1.0.2/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1276 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/PKG-INFO
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      560 2024-03-19 02:01:58.000000 py-glfw-redux-1.0.2/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.407249 py-glfw-redux-1.0.2/build/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/build/py_glfw_redux.egg-info/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18999 2024-03-19 21:54:39.000000 py-glfw-redux-1.0.2/build/py_glfw_redux.egg-info/SOURCES.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.407249 py-glfw-redux-1.0.2/inc/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      885 2024-03-18 04:49:30.000000 py-glfw-redux-1.0.2/inc/list-wrapper.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      588 2024-03-19 00:48:46.000000 py-glfw-redux-1.0.2/inc/modules.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      233 2023-03-09 01:15:58.000000 py-glfw-redux-1.0.2/inc/struct-utility.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      908 2024-03-19 21:38:56.000000 py-glfw-redux-1.0.2/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2024-03-19 21:54:39.440582 py-glfw-redux-1.0.2/setup.cfg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      428 2024-03-19 21:16:09.000000 py-glfw-redux-1.0.2/setup.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/src/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      321 2024-03-18 23:40:04.000000 py-glfw-redux-1.0.2/src/bind-glfw.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7570 2024-03-18 16:54:32.000000 py-glfw-redux-1.0.2/src/constants.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1885 2024-03-19 01:52:53.000000 py-glfw-redux-1.0.2/src/context.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6405 2024-03-18 16:54:55.000000 py-glfw-redux-1.0.2/src/input.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2165 2024-03-18 16:54:55.000000 py-glfw-redux-1.0.2/src/joystick.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2907 2024-03-18 17:43:57.000000 py-glfw-redux-1.0.2/src/monitors.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2144 2024-03-18 16:55:42.000000 py-glfw-redux-1.0.2/src/structs.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9789 2024-03-19 01:16:14.000000 py-glfw-redux-1.0.2/src/windows.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      374 2024-03-18 18:03:29.000000 py-glfw-redux-1.0.2/third-party/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/glfw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1196 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.appveyor.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1275 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.editorconfig
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       44 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.git
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      142 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/glfw/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      147 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.github/CODEOWNERS
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/glfw/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4057 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1449 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/.mailmap
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/glfw/CMake/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1653 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/GenerateMappings.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/Info.plist.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1117 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/cmake_uninstall.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      440 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/glfw3.pc.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      115 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/glfw3Config.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      596 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      588 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/i686-w64-mingw32.cmake
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.410582 py-glfw-redux-1.0.2/third-party/glfw/CMake/modules/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      747 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/modules/FindEpollShim.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      445 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/modules/FindOSMesa.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      606 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      598 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CMake/x86_64-w64-mingw32.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5951 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5328 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/CONTRIBUTORS.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      904 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/LICENSE.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25748 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.413915 py-glfw-redux-1.0.2/third-party/glfw/deps/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/getopt.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2136 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/getopt.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.413915 py-glfw-redux-1.0.2/third-party/glfw/deps/glad/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   326437 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/glad/gl.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81113 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/glad/gles2.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   336197 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/glad/vulkan.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14123 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/linmath.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.413915 py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3111 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/_mingw_dxhelper.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   112560 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/dinput.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7950 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/xinput.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   990698 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/nuklear.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14081 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/nuklear_glfw_gl2.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    71221 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/stb_image_write.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13065 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/tinycthread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15660 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/tinycthread.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.417249 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4636 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/fractional-scale-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4017 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/idle-inhibit-unstable-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15451 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/pointer-constraints-unstable-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6584 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/relative-pointer-unstable-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8232 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/viewporter.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   144896 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/wayland.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9016 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-activation-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7089 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-decoration-unstable-v1.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    60418 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-shell.xml
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.417249 py-glfw-redux-1.0.2/third-party/glfw/docs/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1775 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15396 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/CONTRIBUTING.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   123282 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/Doxyfile.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2024 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/DoxygenLayout.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      460 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/SUPPORT.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16059 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/build.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15323 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/compat.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15112 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/compile.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12135 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/context.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6699 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/extra.css
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4593 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/extra.css.map
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10124 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/extra.scss
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      114 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/footer.html
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1296 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/header.html
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33475 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/input.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4623 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/internal.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24151 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/intro.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1716 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/main.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7900 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/monitor.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20553 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/moving.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14931 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/news.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12464 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/quick.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   110258 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/spaces.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9086 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/vulkan.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    60675 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/docs/window.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.420582 py-glfw-redux-1.0.2/third-party/glfw/examples/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3774 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19484 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/boing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9945 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/gears.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27988 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/glfw.icns
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21630 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/glfw.ico
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       53 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/glfw.rc
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16086 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/heightmap.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4854 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/offscreen.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35989 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/particles.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7146 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/sharing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15210 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/splitview.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5131 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/triangle-opengl.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5264 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/triangle-opengles.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11894 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/wave.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3157 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/examples/windows.c
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.407249 py-glfw-redux-1.0.2/third-party/glfw/include/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.420582 py-glfw-redux-1.0.2/third-party/glfw/include/GLFW/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   241826 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/include/GLFW/glfw3.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21201 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/include/GLFW/glfw3native.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/glfw/src/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13945 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/src/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24776 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_init.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1849 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15740 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_joystick.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19638 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_monitor.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12920 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1890 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1378 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_time.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    60250 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_window.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25670 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29593 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/egl_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      771 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/src/glfw.rc.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23690 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/glx_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14504 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41395 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/input.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35817 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/internal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12404 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/linux_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2322 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/linux_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   256981 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/mappings.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5280 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/mappings.h.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15194 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11919 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/nsgl_context.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14437 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1753 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1424 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5178 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11827 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18608 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/null_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11935 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/osmesa_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6566 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/platform.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6421 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1816 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_module.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3044 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_poll.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1292 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_poll.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3245 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_thread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1674 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_thread.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2206 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1489 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/posix_time.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11947 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/vulkan.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27071 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/wgl_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28467 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26711 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1870 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1822 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_module.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16993 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25101 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3085 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_thread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1956 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_thread.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1911 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1703 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_time.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81112 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/win32_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35148 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    45024 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/wl_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8627 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/wl_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    34576 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/wl_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   102422 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/wl_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    70476 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/x11_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20136 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/x11_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44741 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/x11_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   106290 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/x11_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22943 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/xkb_unicode.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1288 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/src/xkb_unicode.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/glfw/tests/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3920 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4060 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/allocator.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3749 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/clipboard.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14433 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/cursor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3442 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/empty.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22545 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/events.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5739 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/gamma.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    40892 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/glfwinfo.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3919 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/icon.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8696 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/iconify.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9233 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/inputlag.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10852 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/joysticks.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7748 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/monitors.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6165 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/msaa.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6756 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/reopen.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7183 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/tearing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4076 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/threads.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2828 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/timeout.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2112 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/title.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81355 2024-03-18 16:47:39.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/triangle-vulkan.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18678 2024-03-18 16:48:10.000000 py-glfw-redux-1.0.2/third-party/glfw/tests/window.c
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1271 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.appveyor.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      996 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.clang-format
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2605 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.clang-tidy
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2196 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.cmake-format.yaml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1308 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.codespell-ignore-lines
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       48 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.git
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       18 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/pybind11/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      182 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/CODEOWNERS
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15284 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2561 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      328 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      162 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/dependabot.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      116 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/labeler.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       50 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.423915 py-glfw-redux-1.0.2/third-party/pybind11/.github/matchers/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      668 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      645 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.427249 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    34161 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2272 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1491 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/format.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      641 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2628 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2876 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      502 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3706 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       62 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/.readthedocs.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12067 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1684 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      247 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7687 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/README.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      688 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/SECURITY.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.427249 py-glfw-redux-1.0.2/third-party/pybind11/docs/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      607 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/Doxyfile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7417 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/Makefile
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.407249 py-glfw-redux-1.0.2/third-party/pybind11/docs/_static/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.427249 py-glfw-redux-1.0.2/third-party/pybind11/docs/_static/css/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       37 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.427249 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.427249 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3937 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3429 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14283 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3889 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1556 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12371 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9586 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9119 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47796 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8460 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17796 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26729 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15651 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      278 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17161 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9030 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5710 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6377 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9240 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/basics.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2856 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/benchmark.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/benchmark.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   119574 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/changelog.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17090 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/classes.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/docs/cmake/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      273 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/cmake/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25837 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/compiling.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11574 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/conf.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13293 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/faq.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      613 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3277 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/installing.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3079 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/limitations.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    61034 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44653 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    87708 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41121 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    85853 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2647 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/reference.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4577 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/release.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      149 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/requirements.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24035 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.407249 py-glfw-redux-1.0.2/third-party/pybind11/include/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24334 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7750 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    67312 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8458 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      120 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/common.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2096 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28518 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    53480 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5962 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17859 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28221 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    48364 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1625 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      378 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32135 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18442 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      316 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13459 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4731 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5002 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8262 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/gil.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8862 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79725 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9103 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2734 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/options.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   126706 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    98455 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4185 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15477 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29897 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1929 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2765 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/noxfile.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.430582 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      429 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/__init__.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1544 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/__main__.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      228 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/_version.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1207 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/commands.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/py.typed
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17475 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2298 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1495 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/setup.cfg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4855 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/setup.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21733 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5619 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/conftest.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11736 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/constructor_stats.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3578 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1776 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      396 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      926 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/env.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_python_package/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8403 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_setuptools/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4153 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2847 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/local_bindings.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5743 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/object.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6264 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4517 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2685 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      768 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      601 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/requirements.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      855 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_async.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      536 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_async.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10548 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6951 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_buffers.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16025 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17243 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4118 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6549 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_call_policies.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10858 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6796 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_callbacks.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3370 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5691 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_chrono.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24849 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_class.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14757 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_class.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2584 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      673 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1171 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1293 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1685 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      152 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1353 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1163 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1368 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      198 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3831 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      593 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_const_name.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5710 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1551 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26064 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4796 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_copy_move.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7280 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3992 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1259 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1091 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4557 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2423 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19350 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29028 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      473 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10590 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9414 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1798 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1315 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      543 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17396 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      237 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      275 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5722 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_enum.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8939 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_enum.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eval.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1143 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eval.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      119 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_eval_call.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12082 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      399 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_exceptions.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13861 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_exceptions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18155 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16491 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5311 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8507 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3960 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7144 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_iostream.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9444 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13600 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4401 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8054 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22211 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18346 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4121 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_modules.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3963 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_modules.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12305 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11874 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20936 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22886 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21114 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14272 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4487 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9658 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2777 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1847 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9132 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4332 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6719 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2720 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_pickling.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31088 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23892 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_pytypes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21153 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8039 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18898 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9530 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21587 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_stl.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12307 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_stl.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6205 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9804 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4617 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      741 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1855 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_thread.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      826 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_thread.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4501 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_type_caster_pyobject_ptr.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3260 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_type_caster_pyobject_ptr.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      603 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_union.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      148 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_union.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      845 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_unnamed_namespace_a.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1141 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_unnamed_namespace_a.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      341 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_unnamed_namespace_b.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      143 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_unnamed_namespace_b.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1471 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_vector_unique_ptr_member.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      329 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_vector_unique_ptr_member.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22991 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12913 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3226 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2657 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-03-19 21:54:39.437249 py-glfw-redux-1.0.2/third-party/pybind11/tools/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2449 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3105 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11190 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      817 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1423 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/check-style.sh
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      952 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1117 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1031 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/libsize.py
--rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1311 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/make_changelog.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      196 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14449 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7101 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8960 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8361 2024-03-18 16:49:20.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       94 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2104 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1234 2024-03-18 16:48:58.000000 py-glfw-redux-1.0.2/third-party/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.963137 py_glfw_redux-1.1.0/
+-rw-r--r--   0 alagyn    (1000) users      (100)     1175 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) users      (100)     1070 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/LICENSE
+-rw-r--r--   0 alagyn    (1000) users      (100)      168 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     1276 2024-04-16 00:25:33.963137 py_glfw_redux-1.1.0/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) users      (100)      560 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/README.md
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.951137 py_glfw_redux-1.1.0/build/
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.962137 py_glfw_redux-1.1.0/build/py_glfw_redux.egg-info/
+-rw-r--r--   0 alagyn    (1000) users      (100)     7682 2024-04-16 00:25:33.000000 py_glfw_redux-1.1.0/build/py_glfw_redux.egg-info/SOURCES.txt
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.952137 py_glfw_redux-1.1.0/inc/
+-rw-r--r--   0 alagyn    (1000) users      (100)      885 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/inc/list-wrapper.h
+-rw-r--r--   0 alagyn    (1000) users      (100)      646 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/inc/modules.h
+-rw-r--r--   0 alagyn    (1000) users      (100)      233 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/inc/struct-utility.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1151 2024-04-15 22:57:22.000000 py_glfw_redux-1.1.0/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) users      (100)       38 2024-04-16 00:25:33.963137 py_glfw_redux-1.1.0/setup.cfg
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.952137 py_glfw_redux-1.1.0/src/
+-rw-r--r--   0 alagyn    (1000) users      (100)      344 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/bind-glfw.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     5811 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/callbacks.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     7570 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/constants.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     1402 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/context.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     1681 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/input.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     1692 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/joystick.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     2389 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/monitors.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     2145 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/structs.cpp
+-rw-r--r--   0 alagyn    (1000) users      (100)     4240 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/src/windows.cpp
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.952137 py_glfw_redux-1.1.0/third-party/
+-rw-r--r--   0 alagyn    (1000) users      (100)      703 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/third-party/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.951137 py_glfw_redux-1.1.0/third-party/glad/
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.951137 py_glfw_redux-1.1.0/third-party/glad/include/
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.953137 py_glfw_redux-1.1.0/third-party/glad/include/KHR/
+-rw-r--r--   0 alagyn    (1000) users      (100)    11131 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/third-party/glad/include/KHR/khrplatform.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.953137 py_glfw_redux-1.1.0/third-party/glad/include/glad/
+-rw-r--r--   0 alagyn    (1000) users      (100)   299906 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/third-party/glad/include/glad/gl.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.953137 py_glfw_redux-1.1.0/third-party/glad/src/
+-rw-r--r--   0 alagyn    (1000) users      (100)   163913 2024-04-15 22:56:01.000000 py_glfw_redux-1.1.0/third-party/glad/src/gl.c
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.953137 py_glfw_redux-1.1.0/third-party/glfw/
+-rw-r--r--   0 alagyn    (1000) users      (100)     1196 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) users      (100)     1275 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/.editorconfig
+-rw-r--r--   0 alagyn    (1000) users      (100)       44 2024-04-15 23:42:13.000000 py_glfw_redux-1.1.0/third-party/glfw/.git
+-rw-r--r--   0 alagyn    (1000) users      (100)      142 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/.gitattributes
+-rw-r--r--   0 alagyn    (1000) users      (100)     1449 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/.gitignore
+-rw-r--r--   0 alagyn    (1000) users      (100)      384 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/.mailmap
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.954137 py_glfw_redux-1.1.0/third-party/glfw/CMake/
+-rw-r--r--   0 alagyn    (1000) users      (100)     1653 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/GenerateMappings.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)     1297 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/Info.plist.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     1117 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/cmake_uninstall.cmake.in
+-rw-r--r--   0 alagyn    (1000) users      (100)      440 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/glfw3.pc.in
+-rw-r--r--   0 alagyn    (1000) users      (100)      115 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/glfw3Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) users      (100)      596 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)      588 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/i686-w64-mingw32.cmake
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.954137 py_glfw_redux-1.1.0/third-party/glfw/CMake/modules/
+-rw-r--r--   0 alagyn    (1000) users      (100)      747 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/modules/FindEpollShim.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)      445 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/modules/FindOSMesa.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)      606 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)      598 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMake/x86_64-w64-mingw32.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)     5951 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) users      (100)     5328 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/CONTRIBUTORS.md
+-rw-r--r--   0 alagyn    (1000) users      (100)      904 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/LICENSE.md
+-rw-r--r--   0 alagyn    (1000) users      (100)    25748 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/README.md
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.955137 py_glfw_redux-1.1.0/third-party/glfw/deps/
+-rw-r--r--   0 alagyn    (1000) users      (100)     8053 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/getopt.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     2136 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/getopt.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.955137 py_glfw_redux-1.1.0/third-party/glfw/deps/glad/
+-rw-r--r--   0 alagyn    (1000) users      (100)   326437 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/glad/gl.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    81113 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/glad/gles2.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   336197 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/glad/vulkan.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    14123 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/linmath.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.955137 py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/
+-rw-r--r--   0 alagyn    (1000) users      (100)     3111 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/_mingw_dxhelper.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   112560 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/dinput.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     7950 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/xinput.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   990698 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/nuklear.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    14081 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/nuklear_glfw_gl2.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    71221 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/stb_image_write.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    13065 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/tinycthread.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    15660 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/tinycthread.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.956137 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/
+-rw-r--r--   0 alagyn    (1000) users      (100)     4636 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/fractional-scale-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)     4017 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/idle-inhibit-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)    15451 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/pointer-constraints-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)     6584 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/relative-pointer-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)     8232 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/viewporter.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)   144896 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/wayland.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)     9016 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-activation-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)     7089 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-decoration-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) users      (100)    60418 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-shell.xml
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.951137 py_glfw_redux-1.1.0/third-party/glfw/include/
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.956137 py_glfw_redux-1.1.0/third-party/glfw/include/GLFW/
+-rw-r--r--   0 alagyn    (1000) users      (100)   241826 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/include/GLFW/glfw3.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    21201 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/include/GLFW/glfw3native.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.959137 py_glfw_redux-1.1.0/third-party/glfw/src/
+-rw-r--r--   0 alagyn    (1000) users      (100)    13945 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) users      (100)    24776 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_init.m
+-rw-r--r--   0 alagyn    (1000) users      (100)     1849 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_joystick.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    15740 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_joystick.m
+-rw-r--r--   0 alagyn    (1000) users      (100)    19638 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_monitor.m
+-rw-r--r--   0 alagyn    (1000) users      (100)    12920 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1890 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_time.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1378 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_time.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    60250 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_window.m
+-rw-r--r--   0 alagyn    (1000) users      (100)    25670 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/context.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    29593 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/egl_context.c
+-rw-r--r--   0 alagyn    (1000) users      (100)      771 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/glfw.rc.in
+-rw-r--r--   0 alagyn    (1000) users      (100)    23690 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/glx_context.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    14504 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/init.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    41395 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/input.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    35817 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/internal.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    12404 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/linux_joystick.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     2322 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/linux_joystick.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   256981 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/mappings.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     5280 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/mappings.h.in
+-rw-r--r--   0 alagyn    (1000) users      (100)    15194 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/monitor.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    11919 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/nsgl_context.m
+-rw-r--r--   0 alagyn    (1000) users      (100)    14437 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_init.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1753 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_joystick.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1424 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_joystick.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     5178 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_monitor.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    11827 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    18608 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/null_window.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    11935 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/osmesa_context.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     6566 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/platform.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     6421 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1816 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_module.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     3044 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_poll.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1292 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_poll.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     3245 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_thread.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1674 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_thread.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     2206 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_time.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1489 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/posix_time.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    11947 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/vulkan.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    27071 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/wgl_context.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    28467 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_init.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    26711 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_joystick.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1870 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_joystick.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1822 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_module.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    16993 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_monitor.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    25101 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     3085 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_thread.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1956 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_thread.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1911 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_time.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1703 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_time.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    81112 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/win32_window.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    35148 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/window.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    45024 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/wl_init.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     8627 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/wl_monitor.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    34576 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/wl_platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   102422 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/wl_window.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    70476 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/x11_init.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    20136 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/x11_monitor.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    44741 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/x11_platform.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   106290 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/x11_window.c
+-rw-r--r--   0 alagyn    (1000) users      (100)    22943 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/xkb_unicode.c
+-rw-r--r--   0 alagyn    (1000) users      (100)     1288 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/glfw/src/xkb_unicode.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.960137 py_glfw_redux-1.1.0/third-party/pybind11/
+-rw-r--r--   0 alagyn    (1000) users      (100)     1271 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) users      (100)      996 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.clang-format
+-rw-r--r--   0 alagyn    (1000) users      (100)     2605 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.clang-tidy
+-rw-r--r--   0 alagyn    (1000) users      (100)     2196 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.cmake-format.yaml
+-rw-r--r--   0 alagyn    (1000) users      (100)     1308 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 alagyn    (1000) users      (100)       48 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.git
+-rw-r--r--   0 alagyn    (1000) users      (100)       18 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.gitattributes
+-rw-r--r--   0 alagyn    (1000) users      (100)      502 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.gitignore
+-rw-r--r--   0 alagyn    (1000) users      (100)     3706 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 alagyn    (1000) users      (100)       62 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/.readthedocs.yml
+-rw-r--r--   0 alagyn    (1000) users      (100)    12067 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) users      (100)     1684 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/LICENSE
+-rw-r--r--   0 alagyn    (1000) users      (100)      247 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     7687 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/README.rst
+-rw-r--r--   0 alagyn    (1000) users      (100)      688 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/SECURITY.md
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.952137 py_glfw_redux-1.1.0/third-party/pybind11/include/
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.961137 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/
+-rw-r--r--   0 alagyn    (1000) users      (100)    24334 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     7750 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    67312 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     8458 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 alagyn    (1000) users      (100)      120 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     2096 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.961137 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 alagyn    (1000) users      (100)    28518 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    53480 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     5962 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    17859 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    28221 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    48364 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1625 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.961137 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 alagyn    (1000) users      (100)      378 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    32135 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    18442 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 alagyn    (1000) users      (100)      316 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    13459 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     4731 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     5002 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     8262 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     8862 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    79725 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     9103 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     2734 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 alagyn    (1000) users      (100)   126706 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    98455 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.961137 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 alagyn    (1000) users      (100)     4185 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    15477 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 alagyn    (1000) users      (100)    29897 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     1929 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 alagyn    (1000) users      (100)     2765 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/noxfile.py
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.962137 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/
+-rw-r--r--   0 alagyn    (1000) users      (100)      429 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/__init__.py
+-rw-r--r--   0 alagyn    (1000) users      (100)     1544 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/__main__.py
+-rw-r--r--   0 alagyn    (1000) users      (100)      228 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/_version.py
+-rw-r--r--   0 alagyn    (1000) users      (100)     1207 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/commands.py
+-rw-r--r--   0 alagyn    (1000) users      (100)        0 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/py.typed
+-rw-r--r--   0 alagyn    (1000) users      (100)    17475 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 alagyn    (1000) users      (100)     2298 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) users      (100)     1495 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/setup.cfg
+-rw-r--r--   0 alagyn    (1000) users      (100)     4855 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/setup.py
+drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 00:25:33.962137 py_glfw_redux-1.1.0/third-party/pybind11/tools/
+-rw-r--r--   0 alagyn    (1000) users      (100)     2449 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)     3105 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)    11190 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)      817 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 alagyn    (1000) users      (100)     1423 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/check-style.sh
+-rw-r--r--   0 alagyn    (1000) users      (100)      952 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     1117 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 alagyn    (1000) users      (100)     1031 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 alagyn    (1000) users      (100)     1311 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 alagyn    (1000) users      (100)      196 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 alagyn    (1000) users      (100)    14449 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)     7101 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     8960 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)     8361 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 alagyn    (1000) users      (100)       94 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) users      (100)     2104 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 alagyn    (1000) users      (100)     1234 2024-04-15 23:42:14.000000 py_glfw_redux-1.1.0/third-party/pybind11/tools/setup_main.py.in
```

### Comparing `py-glfw-redux-1.0.2/CMakeLists.txt` & `py_glfw_redux-1.1.0/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ${PY_COMPONENTS}
 )
 
 add_subdirectory(third-party)
 
 set(srcs
     src/bind-glfw.cpp
+    src/callbacks.cpp
     src/constants.cpp
     src/context.cpp
     src/input.cpp
     src/joystick.cpp
     src/monitors.cpp
     src/structs.cpp
     src/windows.cpp
@@ -36,17 +37,18 @@
     INTERPROCEDURAL_OPTIMIZATION ON
     VISIBILITY_INLINES_HIDDEN ON
     CXX_STANDARD 17
     OUTPUT_NAME "glfw" # rename to glfw like this so we don't conflict target names
 )
 
 target_link_libraries(pyglfw
-    PRIVATE 
-        pybind11::headers
-        glfw
+    PRIVATE
+    pybind11::headers
+    glfw
+    glad
 )
 
 target_include_directories(pyglfw
     PRIVATE inc
 )
 
 target_compile_definitions(pyglfw
```

### Comparing `py-glfw-redux-1.0.2/LICENSE` & `py_glfw_redux-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/PKG-INFO` & `py_glfw_redux-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-glfw-redux
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python wrapper for GLFW made with PyBind11
 Author: Alagyn
 Project-URL: Homepage, https://github.com/alagyn/py-glfw-redux
 Project-URL: Bug Tracker, https://github.com/alagyn/py-glfw-redux/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-glfw-redux-1.0.2/README.md` & `py_glfw_redux-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/inc/list-wrapper.h` & `py_glfw_redux-1.1.0/inc/list-wrapper.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/inc/modules.h` & `py_glfw_redux-1.1.0/inc/modules.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #pragma once
 
+#include <glad/gl.h>
+
 #include <GLFW/glfw3.h>
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 using namespace pybind11::literals;
 
 #define QUICK(func) m.def(#func, glfw##func);
@@ -24,8 +26,9 @@
 //void init_internal(py::module& m);
 void init_constants(py::module& m);
 void init_structs(py::module& m);
 void init_context(py::module& m);
 void init_monitors(py::module& m);
 void init_windows(py::module& m);
 void init_input(py::module& m);
-void init_joystick(py::module& m);
+void init_joystick(py::module& m);
+void init_callbacks(py::module& m);
```

### Comparing `py-glfw-redux-1.0.2/src/constants.cpp` & `py_glfw_redux-1.1.0/src/constants.cpp`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/src/joystick.cpp` & `py_glfw_redux-1.1.0/src/joystick.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 #include <modules.h>
 
 #include <list-wrapper.h>
 
 static py::object joystickCallback;
 
-void joystickCallbackFunc(int jid, int event)
-{
-    if(!joystickCallback.is_none())
-    {
-        joystickCallback(jid, event);
-    }
-}
-
 void init_joystick(py::module& m)
 {
     joystickCallback = py::none();
 
     m.def(
         "JoystickPresent",
         [](int jid)
@@ -68,25 +60,12 @@
         [](int jid)
         {
             return static_cast<bool>(glfwJoystickIsGamepad(jid));
         },
         "jid"_a
     );
 
-    m.def(
-        "SetJoysticksCallback",
-        [](GLFWwindow* window, py::object callback)
-        {
-            py::object out = joystickCallback;
-            joystickCallback = callback;
-            glfwSetJoystickCallback(joystickCallbackFunc);
-            return out;
-        },
-        "window"_a,
-        "callback"_a
-    );
-
     m.def("UpdateGamepadMappings", glfwUpdateGamepadMappings, "string"_a);
     m.def("GetGamepadName", glfwGetGamepadName, "jid"_a);
     // TODO this might be need to be a lambda
     m.def("GetGamepadState", glfwGetGamepadName, "jid_a", "state"_a);
 }
```

### Comparing `py-glfw-redux-1.0.2/src/monitors.cpp` & `py_glfw_redux-1.1.0/src/monitors.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,12 @@
 #include <list-wrapper.h>
 #include <modules.h>
 
-static py::object monitorCallback;
-
-void monitorSetCallbackFunc(GLFWmonitor* monitor, int event)
-{
-    if(!monitorCallback.is_none())
-    {
-        monitorCallback(monitor, event);
-    }
-}
-
 void init_monitors(py::module& m)
 {
-    monitorCallback = py::none();
-
     initListWrapper<GLFWmonitor*>(m, "ListWrapperMonitor");
 
     m.def(
         "GetMonitors",
         []()
         {
             int count;
@@ -74,26 +62,14 @@
     );
 
     m.def("GetMonitorName", glfwGetMonitorName, "monitor"_a);
 
     // TODO glfwSetMonitorUserPointer? Might not be useful
     // glfwGetMonitorUserPointer
 
-    m.def(
-        "SetMonitorCallback",
-        [](py::object callback)
-        {
-            py::object out = monitorCallback;
-            monitorCallback = callback;
-            glfwSetMonitorCallback(monitorSetCallbackFunc);
-            return out;
-        },
-        "callback"_a
-    );
-
     initListWrapper<GLFWvidmode>(m, "ListWrapperVidmode");
 
     m.def(
         "GetVideoModes",
         [](GLFWmonitor* monitor)
         {
             int count;
```

### Comparing `py-glfw-redux-1.0.2/src/structs.cpp` & `py_glfw_redux-1.1.0/src/structs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+#include <modules.h>
+
 #include <GLFW/glfw3.h>
 
 #include <list-wrapper.h>
-#include <modules.h>
 #include <struct-utility.h>
 
 namespace py = pybind11;
 
 void init_structs(pybind11::module& m)
 {
     initListWrapper<unsigned short>(m, "ListWrapperUS");
```

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/.appveyor.yml` & `py_glfw_redux-1.1.0/third-party/glfw/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/.editorconfig` & `py_glfw_redux-1.1.0/third-party/glfw/.editorconfig`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/.gitignore` & `py_glfw_redux-1.1.0/third-party/glfw/.gitignore`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/GenerateMappings.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/GenerateMappings.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/Info.plist.in` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/Info.plist.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/cmake_uninstall.cmake.in` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/i686-w64-mingw32.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/i686-w64-mingw32.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/modules/FindEpollShim.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/modules/FindEpollShim.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMake/x86_64-w64-mingw32.cmake` & `py_glfw_redux-1.1.0/third-party/glfw/CMake/x86_64-w64-mingw32.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CMakeLists.txt` & `py_glfw_redux-1.1.0/third-party/glfw/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/CONTRIBUTORS.md` & `py_glfw_redux-1.1.0/third-party/glfw/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/LICENSE.md` & `py_glfw_redux-1.1.0/third-party/glfw/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/README.md` & `py_glfw_redux-1.1.0/third-party/glfw/README.md`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/getopt.c` & `py_glfw_redux-1.1.0/third-party/glfw/deps/getopt.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/getopt.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/getopt.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/glad/gl.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/glad/gl.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/glad/gles2.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/glad/gles2.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/glad/vulkan.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/glad/vulkan.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/linmath.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/linmath.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/_mingw_dxhelper.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/_mingw_dxhelper.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/dinput.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/dinput.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/mingw/xinput.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/mingw/xinput.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/nuklear.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/nuklear.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/nuklear_glfw_gl2.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/nuklear_glfw_gl2.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/stb_image_write.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/tinycthread.c` & `py_glfw_redux-1.1.0/third-party/glfw/deps/tinycthread.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/tinycthread.h` & `py_glfw_redux-1.1.0/third-party/glfw/deps/tinycthread.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/fractional-scale-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/fractional-scale-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/idle-inhibit-unstable-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/idle-inhibit-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/pointer-constraints-unstable-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/pointer-constraints-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/relative-pointer-unstable-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/relative-pointer-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/viewporter.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/viewporter.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/wayland.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/wayland.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-activation-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-activation-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-decoration-unstable-v1.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-decoration-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/deps/wayland/xdg-shell.xml` & `py_glfw_redux-1.1.0/third-party/glfw/deps/wayland/xdg-shell.xml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/include/GLFW/glfw3.h` & `py_glfw_redux-1.1.0/third-party/glfw/include/GLFW/glfw3.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/include/GLFW/glfw3native.h` & `py_glfw_redux-1.1.0/third-party/glfw/include/GLFW/glfw3native.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/CMakeLists.txt` & `py_glfw_redux-1.1.0/third-party/glfw/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_init.m` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_init.m`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_joystick.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_joystick.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_joystick.m` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_joystick.m`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_monitor.m` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_monitor.m`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_time.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_time.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_time.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_time.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/cocoa_window.m` & `py_glfw_redux-1.1.0/third-party/glfw/src/cocoa_window.m`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/context.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/context.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/egl_context.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/egl_context.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/glfw.rc.in` & `py_glfw_redux-1.1.0/third-party/glfw/src/glfw.rc.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/glx_context.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/glx_context.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/init.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/init.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/input.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/input.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/internal.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/internal.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/linux_joystick.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/linux_joystick.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/linux_joystick.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/linux_joystick.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/mappings.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/mappings.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/mappings.h.in` & `py_glfw_redux-1.1.0/third-party/glfw/src/mappings.h.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/monitor.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/monitor.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/nsgl_context.m` & `py_glfw_redux-1.1.0/third-party/glfw/src/nsgl_context.m`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_init.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_init.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_joystick.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_joystick.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_joystick.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_joystick.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_monitor.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_monitor.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/null_window.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/null_window.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/osmesa_context.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/osmesa_context.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/platform.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/platform.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_module.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_module.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_poll.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_poll.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_poll.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_poll.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_thread.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_thread.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_thread.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_thread.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_time.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_time.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/posix_time.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/posix_time.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/vulkan.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/vulkan.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/wgl_context.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/wgl_context.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_init.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_init.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_joystick.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_joystick.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_joystick.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_joystick.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_module.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_module.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_monitor.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_monitor.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_thread.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_thread.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_thread.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_thread.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_time.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_time.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_time.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_time.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/win32_window.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/win32_window.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/window.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/window.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/wl_init.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/wl_init.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/wl_monitor.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/wl_monitor.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/wl_platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/wl_platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/wl_window.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/wl_window.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/x11_init.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/x11_init.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/x11_monitor.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/x11_monitor.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/x11_platform.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/x11_platform.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/x11_window.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/x11_window.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/xkb_unicode.c` & `py_glfw_redux-1.1.0/third-party/glfw/src/xkb_unicode.c`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/glfw/src/xkb_unicode.h` & `py_glfw_redux-1.1.0/third-party/glfw/src/xkb_unicode.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.appveyor.yml` & `py_glfw_redux-1.1.0/third-party/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.clang-format` & `py_glfw_redux-1.1.0/third-party/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.clang-tidy` & `py_glfw_redux-1.1.0/third-party/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.cmake-format.yaml` & `py_glfw_redux-1.1.0/third-party/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.codespell-ignore-lines` & `py_glfw_redux-1.1.0/third-party/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/.pre-commit-config.yaml` & `py_glfw_redux-1.1.0/third-party/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/CMakeLists.txt` & `py_glfw_redux-1.1.0/third-party/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/LICENSE` & `py_glfw_redux-1.1.0/third-party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/README.rst` & `py_glfw_redux-1.1.0/third-party/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/SECURITY.md` & `py_glfw_redux-1.1.0/third-party/pybind11/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/attr.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/buffer_info.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/cast.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/chrono.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/complex.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/class.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/common.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/descr.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/init.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/internals.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/type_caster_base.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/detail/typeid.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/matrix.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eigen/tensor.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/embed.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/eval.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/functional.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/gil.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/iostream.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/numpy.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/operators.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/options.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/pybind11.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/pytypes.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl/filesystem.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/stl_bind.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `py_glfw_redux-1.1.0/third-party/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/noxfile.py` & `py_glfw_redux-1.1.0/third-party/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/pybind11/__main__.py` & `py_glfw_redux-1.1.0/third-party/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/pybind11/commands.py` & `py_glfw_redux-1.1.0/third-party/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/pybind11/setup_helpers.py` & `py_glfw_redux-1.1.0/third-party/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/pyproject.toml` & `py_glfw_redux-1.1.0/third-party/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/setup.cfg` & `py_glfw_redux-1.1.0/third-party/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/setup.py` & `py_glfw_redux-1.1.0/third-party/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/FindCatch.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/FindEigen3.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/FindPythonLibsNew.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/JoinPaths.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/check-style.sh` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/cmake_uninstall.cmake.in` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/libsize.py` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/make_changelog.py` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Common.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Config.cmake.in` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11NewTools.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/pybind11Tools.cmake` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/setup_global.py.in` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `py-glfw-redux-1.0.2/third-party/pybind11/tools/setup_main.py.in` & `py_glfw_redux-1.1.0/third-party/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

