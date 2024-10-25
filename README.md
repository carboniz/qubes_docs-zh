# Introduction-介绍
## What
Qubes OS 利用基于Xen虚拟化来创建和管理称为qubes的隔离隔间。
- [ ] Xen-based
## Features
- 模板系统： app qubes 共享根文件系统  
- disposables：关闭即自毁的一次性用品  
- 设备隔离：隔离网卡和usb设备
- [ ] split GPG 分割GPG,保证私钥安全;
- [ ] CTAP proxy to use two-factor authentication devices;
---
# Getting started
## 基础
- app qubes 基于 template-模板，不得修改模板，在A模板安装某应用，更新后基于A的app qubes都可运行该程序;
- service qube：管理网络连接，usb设备;
- admin qube: dom0, 拥有最高权限，无网络连接，仅用于运行桌面环境。
## 色彩 & 安全
不同颜色追踪各qube的可信度，一般，红色表示危险，黑色表示安全。完全可自由定制颜色含义。
## 用户界面
![picture](https://www.qubes-os.org/attachment/doc/r4.0-taskbar.png)
- App Menu：应用程序菜单，打开qubes，设置。
- Task Bar：打开和隐藏窗口。
- Space：虚拟桌面的界面，无隔离属性。
- Tray：一些小部件。

Qubes OS 独有的小部件
![picture](https://www.qubes-os.org/attachment/doc/r4.1-widgets.png)
- Whonix SDWDate：管理Tor连接。
- Clipboard：从dom0复制文本。
- Devices：管理连接到qubes的设备。
- Disk Space Monitor：显示磁盘存储空间
- Domains：管理qubes,打开/关闭它们及监视RAM和CPU使用情况。
- Updater：有可用更新时提醒，并辅助安装。
## dom0 termianl
1. 右击桌面，open terminal here
2. Alt + F3 搜索 xfce terminal
3. App Menu -> 设置 -> other -> xfce terminal
## 添加，删除，列出qubes
1. Qube Manager
2. command: `qvm-create` `qvm-remove` `qvm-ls`
## 安全习惯
*保持更新* *定期备份*
---
# How-To 操作指南


