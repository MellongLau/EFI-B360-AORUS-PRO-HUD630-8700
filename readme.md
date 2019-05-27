## 硬件配置
**CPU**  I7 8700  
**主板**  技嘉 B360 M AORUS PRO 小雕  
**内存**  海盗船 DDR4 3200 16G  
**固态硬盘**  SN750 M.2 Nvme 1TB  
**WIFI和蓝牙**  BCM943602CS2 两天线版  
**显示器**  Dell 24寸  
**机箱** 追风者416PSTG钢化玻璃RGB静音豪华版  

## 系统版本
macOS Mojave 10.14.5

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

## 未来更新
内存增加一条16G组合为双通道
加独立显卡RX580或者RX590组合为双通道
加Dell 27寸4K显示器实现retina显示

## 问题及解决方法
1. 两天线BCM943602CS网速变慢，要重启才恢复，每次睡眠唤醒后网速变慢，蓝牙出现问题容易卡顿。  
参看远景论坛http://bbs.pcbeta.com/viewthread-1811853-1-1.html
去掉Energy saver的 Wake for internect access, 去掉蓝牙的高级选项 Allow bluetooth device to wake this computer.
如果问题还没解决就确认是否有使用AirportBrcmFixup.kext这个kext，没有的话加上就好了。

2. 安装第二次启动剩余15分钟自动重启问题，无法安装.  
这个问题比较奇怪，用的USB2.0，但是第二次重启后还是不行，直接拔了插到USB3.0的接口重启安装一切正常。

## 特别鸣谢
感谢[@ParkinWu](https://github.com/ParkinWu/EFI-B360-AORUS-PRO-HUD630-8700)分享的EFI文件。
