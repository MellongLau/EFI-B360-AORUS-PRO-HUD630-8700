## 硬件配置
**CPU** I7 8700  
**主板** 技嘉 B360 M AORUS PRO 小雕  
**内存** 海盗船 DDR4 3200 32G（16GX2双通道，只能超频到2666）  
**硬盘** MacOS 三星860 EVO SSD 500G, Win10 SN750 M.2 Nvme 1TB, 资料盘 东芝4T 7200  
**WIFI和蓝牙** BCM943602CS2 两天线版  
**显卡** 蓝宝石 RX590 8G 超白金  
**显示器** Dell 24寸 + Dell U2718Q 4K  
**机箱** 追风者416PSTG钢化玻璃RGB静音豪华版  

## 系统版本
macOS Catalina 10.15.5

## 完美驱动
声卡  
网卡  
CPU变频  
休眠和唤醒  
DP输出口(可4K)  
USB3.0  
WIFI和蓝牙  

## 安装前BIOS设置
硬盘模式调整为 AHCI  
开启支持 UEFI 启动，一般默认是开启的  
关闭VT-d，安完完系统后，再开启  
关闭Secure Boot Mode  
OS Type选项，设置为 Other OS  
关闭IO SerialPort  
设置 XHCI Handoff 为 开启  

## 安装后工具
Hackintool  
iStat Menus  
Disk Spped Test  
Geekbench 4  
Clover Configurator  

## 未来更新
* 改用 OpenCore 引导
* 尝试升级到 macOS Big Sur 10.16 Beta
* 加 16GX2 内存，达到64G 内存
* 加 1T 三星860 EVO SSD 和 4T 西部数据64M蓝盘硬盘
* 加小米显示器挂灯和明基显示器挂灯

## 问题及解决方法
1. 两天线BCM943602CS网速变慢，要重启才恢复，每次睡眠唤醒后网速变慢，蓝牙出现问题容易卡顿。  
参看[远景论坛](http://bbs.pcbeta.com/viewthread-1811853-1-1.html)
去掉Energy saver的 Wake for internect access, 去掉蓝牙的高级选项 Allow bluetooth device to wake this computer.
如果问题还没解决就确认是否有使用AirportBrcmFixup.kext这个kext，没有的话加上就好了。

2. 安装第二次启动剩余15分钟自动重启问题，无法安装.  
这个问题比较奇怪，用的USB2.0，但是第二次重启后还是不行，直接拔了插到USB3.0的接口重启安装一切正常。

3. Win10使用SN750可能出现蓝屏重启，特别是冷启动的时候更容易蓝屏。
解决方法是安装主板官网最新驱动，关闭win10的快速启动功能（在电源设置里面关闭）。

## 特别鸣谢
感谢[@ParkinWu](https://github.com/ParkinWu/EFI-B360-AORUS-PRO-HUD630-8700)分享的EFI文件。  
感谢[@YellBinn](https://github.com/YellBinn/GIGABYTE-B360M-AORUS-PRO-8400-EFI-Hackintosh)提供的安装资料。
