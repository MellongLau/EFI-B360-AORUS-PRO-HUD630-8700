1. 两天线BCM943602CS网速变慢，要重启才恢复，每次睡眠唤醒后网速变慢，蓝牙出现问题容易卡顿。
参看远景论坛http://bbs.pcbeta.com/viewthread-1811853-1-1.html
去掉Energy saver的 Wake for internect access, 去掉蓝牙的高级选项 Allow bluetooth device to wake this computer.
如果问题还没解决就确认是否有使用AirportBrcmFixup.kext这个kext，没有的话加上就好了。

2. 安装第二次启动剩余15分钟自动重启问题，无法安装
这个问题比较奇怪，用的USB2.0，但是第二次重启后还是不行，直接拔了插到USB3.0的接口重启安装一切正常。
