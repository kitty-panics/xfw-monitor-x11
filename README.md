# xfw-monitor-x11

输出 `~/.config/xfce4/desktop/icons.screen0.yaml` 所需的 Monitor 信息。

## 参考

代码 Dump 自 [libxfce4windowing] 项目的 `xfw-monitor.c`/`xfw-monitor-x11.c` 文件。

## 编译

```Bash
gcc xfw-monitor-x11.c $(pkg-config --cflags --libs x11 xrandr) -lcrypto -o xfw-monitor-x11
```

## 使用

```Bash
./xfw-monitor-x11     # 输出每个已连接显示器信息
./xfw-monitor-x11 -c  # 输出 xfdesktop 所需的前置配置片段
```
```
