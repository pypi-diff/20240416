# Comparing `tmp/lyyprocess-1.5.tar.gz` & `tmp/lyyprocess-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyprocess-1.5.tar", last modified: Thu Mar 21 05:06:35 2024, max compression
+gzip compressed data, was "lyyprocess-1.6.tar", last modified: Tue Apr 16 14:34:09 2024, max compression
```

## Comparing `lyyprocess-1.5.tar` & `lyyprocess-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 05:06:35.858294 lyyprocess-1.5/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyprocess-1.5/LICENSE
--rw-rw-rw-   0        0        0      157 2024-03-21 05:06:35.858294 lyyprocess-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyprocess-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 05:06:35.856292 lyyprocess-1.5/lyyprocess.egg-info/
--rw-rw-rw-   0        0        0      157 2024-03-21 05:06:35.000000 lyyprocess-1.5/lyyprocess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-03-21 05:06:35.000000 lyyprocess-1.5/lyyprocess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 05:06:35.000000 lyyprocess-1.5/lyyprocess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-21 05:06:35.000000 lyyprocess-1.5/lyyprocess.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 05:06:35.000000 lyyprocess-1.5/lyyprocess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13117 2024-03-21 05:06:19.000000 lyyprocess-1.5/lyyprocess.py
--rw-rw-rw-   0        0        0       42 2024-03-21 05:06:35.858294 lyyprocess-1.5/setup.cfg
--rw-rw-rw-   0        0        0      277 2024-03-21 05:06:34.000000 lyyprocess-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:34:09.084454 lyyprocess-1.6/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyprocess-1.6/LICENSE
+-rw-rw-rw-   0        0        0      157 2024-04-16 14:34:09.083428 lyyprocess-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyprocess-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 14:34:09.082414 lyyprocess-1.6/lyyprocess.egg-info/
+-rw-rw-rw-   0        0        0      157 2024-04-16 14:34:08.000000 lyyprocess-1.6/lyyprocess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-16 14:34:08.000000 lyyprocess-1.6/lyyprocess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:34:08.000000 lyyprocess-1.6/lyyprocess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 14:34:08.000000 lyyprocess-1.6/lyyprocess.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 14:34:08.000000 lyyprocess-1.6/lyyprocess.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14288 2024-04-16 14:34:02.000000 lyyprocess-1.6/lyyprocess.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:34:09.084454 lyyprocess-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      277 2024-04-16 14:34:07.000000 lyyprocess-1.6/setup.py
```

### Comparing `lyyprocess-1.5/LICENSE` & `lyyprocess-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyprocess-1.5/lyyprocess.py` & `lyyprocess-1.6/lyyprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,129 @@
 import psutil
 import socket
 import subprocess
 import time
-import os
-import wmi
+import os,sys
 import threading
-import win32gui
-import psutil
-import re
-import pygetwindow as gw
-import win32process
 
 
-def 重复线程检测(self, func):
-    for thread in threading.enumerate():
-        if thread.name == func.__name__:
+def is_window_exists_by_title(title):
+    import win32gui
+    try:
+        # 定义回调函数，用于枚举所有窗口
+        def enum_windows_proc(hwnd, lParam):
+            if win32gui.IsWindowVisible(hwnd) and win32gui.GetWindowText(hwnd) == title:
+                lParam.append(hwnd)
             return True
-    return False
 
+        # 创建一个空列表，用于存储找到的窗口句柄
+        hwnds = []
+        # 枚举所有顶级窗口，并对每个窗口执行回调函数
+        win32gui.EnumWindows(enum_windows_proc, hwnds)
 
-def check_process_type(process_name):
-    for proc in psutil.process_iter(["pid", "name", "username", "status"]):
-        if proc.info["name"] == process_name:
-            if proc.info["username"] == "NT AUTHORITY\\SYSTEM":
-                return "以Windows服务运行"
-            else:
-                return "以用户交互界面运行"
-    return f"进程列表中找不到该程序{process_name},可能未运行"
+        # 如果列表不为空，说明找到了具有指定标题的窗口
+        return len(hwnds) > 0
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return False
 
 
-def get_top_window(debug=False):
-    # log("# 获取最顶层程序的窗口句柄")
-    hwnd = win32gui.GetForegroundWindow()
-    # log("# 获取窗口标题from hwnd"+str(hwnd))
-    if hwnd < 1:
-        if debug:
-            print("hwnd<1,return")
-        time.sleep(1)
-        return
-    hwnd = hwnd[1] if isinstance(hwnd, list) else hwnd
-    title = win32gui.GetWindowText(hwnd)
-
-    # log("# 获取pidfrom hwnd"+str(hwnd))
-    pid = win32process.GetWindowThreadProcessId(hwnd)[1]
-
-    # log("# 获取进程名from pid"+str(pid))
-    process_name = psutil.Process(pid).name()
-    # log("# 获取进程名finish")
+def is_self_already_running(if_exit=True, debug=False):
+    """
+    判断程序自身是否已经运行，如果参数if_exit为真，则直接退出。
+    """
+    current_process = psutil.Process()
     if debug:
-        print("top win hwd=", hwnd, title, end=" ")
-    return hwnd, title, process_name
+        print(current_process.name(), current_process.pid)
+    for proc in psutil.process_iter(["pid", "name"]):
+        if debug:
+            print(proc.info["name"], proc.info["pid"])
+        # 检查进程名称和PID是否与当前进程相同
+        if proc.info["name"] != "python.exe" and proc.info["name"] == current_process.name() and proc.pid != current_process.pid:
+            if if_exit:
+                sys.exit()
+            return True
+    return False
 
 
-def if_process_is_top(exe_name, debug=False):
-    try:
-        hwnd, window_title, process_name = get_top_window()
-    except Exception as e:
-        print("if_tdx_top:" + str(e))
-        return
-    # 判断窗口标题是否包含“通达信”且进程名为“tdx.exe”
-    if exe_name.lower() in process_name.lower():
-        if debug:
-            print("通达信i is true")
-        return True
-    else:
-        if debug:
-            print("通达信 is false`" + window_title)
-        return False
+def exit_program(root=None):
+    """
+    退出程序，关闭 Tkinter 窗口并终止程序运行。
 
+    :param root: Tkinter 的根窗口对象
+    """
+    if root is not None:
+        root.quit()  # 关闭 Tkinter 窗口
+    sys.exit()   # 终止程序运行
 
-def xxx(exe_name, debug=False):
-    if debug:
-        print("enter if_process_is_top")
-    for proc in psutil.process_iter(["pid", "name", "create_time", "cpu_percent"]):
-        print(proc.info["name"])
-        if proc.info["name"].lower() == exe_name.lower():
-            if proc.info["pid"] == psutil.Process().pid:
-                return True
-            break
+
+
+def open_config_file(file_to_open=None):
+    """打开包含任务信息的文件"""
+    os.startfile(file_to_open)  # 在默认程序中打开文件序中打开文件
+
+def open_file_in_new_thread(filepath):
+
+    def edit_file(filepath):
+        subprocess.run(["notepad.exe", filepath])
+
+    thread = threading.Thread(target=edit_file, args=(filepath,))
+    thread.start()
+
+
+def monitor_and_start_thread(thread, target, args):
+    """
+    检查线程是否在运行，如果没有运行，则启动它。
+    
+    :param thread: 要监测的线程对象
+    :param target: 线程目标函数
+    :param args: 传递给目标函数的参数
+    """
+    if not thread.is_alive():
+        # 线程未在运行，启动线程
+        thread = threading.Thread(target=target, args=args, daemon=True)
+        thread.start()
+        print("线程已启动")
+    else:
+        print("线程正在运行")
+
+def is_program_running(exe_file_name):
+    """检查指定的程序是否正在运行"""
+    if ".exe" not in exe_file_name:
+        exe_file_name += ".exe"
+    for process in psutil.process_iter(["name"]):
+        if process.info["name"].lower() == exe_file_name.lower():
+            return True
     return False
 
+def start_programe_in_new_process(full_path):
+        # Windows平台的创建新进程组标志
+    CREATE_NEW_PROCESS_GROUP, DETACHED_PROCESS = 0x00000200, 0x00000008
+
+    subprocess.Popen([full_path], creationflags=DETACHED_PROCESS | CREATE_NEW_PROCESS_GROUP)
+
+def restart_program(programe_path, program_name):
+    try:
+        # 结束进程
+        subprocess.run(["taskkill", "/f", "/im", program_name], check=True)
+        print(f"Program {program_name} has been terminated.")
+    except subprocess.CalledProcessError as e:
+        print(f"报错但应该是正常现象。有可能该进程本来就结束了，所以才需要修复。错误信息为：Error terminating program {program_name}: {e}")
+
+    try:
+        # 等待一段时间，确保进程已经完全结束
+        time.sleep(2)
+        # 重新启动进程
+        # 假设程序在系统的PATH中，或者提供完整的路径
+        # subprocess.run([programe_path + "/" + program_name], check=True)
+        program_path = programe_path + "/" + program_name
+        start_programe_in_new_process(program_path)
+        print(f"Program {program_name} has been restarted.")
+    except subprocess.CalledProcessError as e:
+        print(f"Error starting program {program_name}: {e}")
 
 def open_directory(dir_name):
     subprocess.Popen(r"explorer " + dir_name)
 
 
 def open_file_in_new_thread(filepath):
 
@@ -213,19 +253,49 @@
                     pid = conn.pid
                     process = psutil.Process(pid)
                     print(f"# 占用端口的进程名：{process.name()}，进程路径：{process.exe()}")
                     return process.name(), process.exe()
     return None, None
 
 
+
+def kill_process_by_path(executable_path):
+    for proc in psutil.process_iter(["pid", "exe"]):
+        if proc.info["exe"] == executable_path:
+            try:
+                proc.kill()
+                print(f"已结束进程 PID: {proc.pid}")
+            except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess) as e:
+                print(f"无法结束进程 PID: {proc.pid}, 错误: {e}")
+
+
+
+
+def kill_process_by_name(path):
+    for proc in psutil.process_iter(["name"]):
+        if proc.info["name"] == name:
+            proc.kill()
+
 def kill_process_by_name(name):
     for proc in psutil.process_iter(["name"]):
         if proc.info["name"] == name:
             proc.kill()
 
+def kill_process_by_title_and_exe(window_title, exe_name):
+
+    try:
+        # 使用 wmic 命令查询具有特定窗口标题的进程的进程ID
+        result = subprocess.run(["wmic", "process", "where", f"name='{exe_name}' and windowtitle='{window_title}'", "get", "/value"], capture_output=True, text=True, check=True)
+        pid = result.stdout.strip()  # 获取进程ID
+
+        # 使用 taskkill 命令结束特定的进程
+        subprocess.run(["taskkill", "/f", "/pid", pid], check=True)
+        print(f"进程 {pid} 已被结束。")
+    except subprocess.CalledProcessError as e:
+        print(f"无法结束进程: {e}")
 
 def terminate_process_using_port(port):
     try:
         command = f"netstat -ano | findstr :{port}"
         output = subprocess.check_output(command, shell=True, text=True)
         lines = output.strip().split("\n")
         for line in lines:
@@ -274,41 +344,15 @@
     #     for thread_id, thread_obj in threading._active.items():
     #         if thread_obj.ident != main_thread.ident:
     #             #print(f"  Thread ID: {thread_obj.ident}")
     print("子线程数量为：", len(children))
     return len(children)
 
 
-def get_hwnd(process_name, debug=False):
-    for proc in psutil.process_iter(["pid", "name"]):
-        if debug:
-            print(proc.as_dict(attrs=["pid", "name"])["name"], process_name.lower())
-        if debug:
-            print(".", end="", flush=True)
-        try:
-            proc_info = proc.as_dict(attrs=["pid", "name"])
-            if process_name.lower() in proc_info["name"].lower():
-
-                pid = proc_info["pid"]
-                if debug:
-                    print("get the needed process, 要找的exe名字(", process_name + ")对应的pid=", pid)
-                result = gw.getWindowsWithTitle(f"pid={pid}")
-                if len(result) > 0:
-                    hwnd = result[0].hwnd
-                    return hwnd
-            else:
-                if debug:
-                    print(".", end="", flush=True)
-                # if debug: print("当前exe=",proc.as_dict(attrs=["pid", "name"])["name"],"需要找的exe=",process_name.lower() )
-        except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
-            pass
-    return None
-
-
-def get_pid(process_name):
+def get_hwnd(process_name):
     for proc in psutil.process_iter(["pid", "name"]):
         try:
             proc_info = proc.as_dict(attrs=["pid", "name"])
             if process_name.lower() in proc_info["name"].lower():
                 return proc_info["pid"]
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
@@ -318,45 +362,17 @@
     if process is not None:
         process.nice(psutil.HIGH_PRIORITY_CLASS)
         print(f"已将进程 {process.pid} 置顶")
     else:
         print("未找到名为 'kingtrade' 的进程")
 
 
-# 示例：将窗口句柄为12345的窗口放在最上层
-import win32gui, win32con
-
-
-def set_window_top(hwnd):
-    print(hwnd)
-    win32gui.SetWindowPos(hwnd, win32con.HWND_TOPMOST, 0, 0, 0, 0, win32con.SWP_NOMOVE | win32con.SWP_NOSIZE)
-
-
-# 获取指定句柄的窗口标题
-def get_window_title(hwnd):
-    return win32gui.GetWindowText(hwnd)
-
-
-# 根据窗口标题找到句柄，并置顶窗口
-def find_and_set_top_window(title):
-    # 当前看起来不生效。不得不用pywinauto
-    def callback(hwnd, hwnds):
-        if win32gui.IsWindowVisible(hwnd) and title in get_window_title(hwnd):
-            set_window_top(hwnd)
-
-    win32gui.EnumWindows(callback, None)
 
 
 if __name__ == "__main__":
-
-    time.sleep(3)
-    print(if_process_is_top("tdxw.exe", debug=True))  # 应输出False，因为notepad不是活动窗口
-
-    time.sleep(3333)
-
     print(check_port_in_use(3306))
     kill_process_by_name("notepad.exe")
 
     exit()
     task_dict = {"jiepan": "D:/Soft/_lyytools/_jiepan/_jiepan.exe", "gui-only": "D:/Soft/_lyytools/gui-only/gui-only.exe", "kingtrader": "D:/Soft/_Stock/KTPro/A.点我登录.exe"}
     stopped = check_processes(task_dict)
     print("stopped=", stopped)
```

