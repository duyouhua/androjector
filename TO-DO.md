###TO-DO

1. 优化流程
2. 降低画质

####1 优化流程

现有两套方案：

1. 设备端取得root权限后完全使用PC端adb控制（screencap + pull + show）（ver 1）
2. 设备端取得root权限后使用Android Service维护图像序列，PC端仅pull + show

####2 降低画质

现有两套方案：

1. 运行screencap 获得raw数据后在设备上缩小为1/4（push到设备中后使用PC端控制，C + 管道，bmp + gzip）（ver 2.2）
2. 利用ddmlib.jar重写PC端程序获得截图（Java）

（ver 3将尝试使用流程 1）
