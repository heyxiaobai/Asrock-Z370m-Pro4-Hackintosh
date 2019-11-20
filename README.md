### EFI概述

> 通过[小兵](https://blog.daliansky.net/macOS-Catalina-10.15.1-19B88-Release-version-with-Clover-5098-original-image-Double-EFI-Version.html)的EFI文件进行精简优化，已停止开发，转至[OpenCore引导](https://github.com/heyxiaobai/Asrock-Z370m-Pro4-Hackintosh/)

Mac 版本：10.15.1

Clover 版本：5098

更新日期：2019-11-20



### 配置清单

| 类型       | 型号                   | 价格 |
| ---------- | ---------------------- | ---- |
| 主板       | 华擎 Z370M Pro4        | 420  |
| CPU        | i3 9100F（散片）+ 散热 | 500  |
| 显卡       | 蓝宝石 RX 570（矿卡）  | 300  |
| 内存条     | 光威 DDR4 16G 2666MHz  | 270  |
| 硬盘       | 西数 M2 120G           | 100  |
| 网卡、蓝牙 | BCM943602cs            | 200  |
| 电源       | 长城 500W（二手）      | 100  |
| 机箱       | Thermeltake s3         | 100  |
| 显示器     | 三星 1080P（二手）     | 150  |
| 总         |                        | 2140 |

> 注：该CPU没有核显



### 功能测试

##### 正常使用的功能

* 前后端声音输入输出
* USB2.0、3.0端口
* 有线网络
* WIFI、蓝牙、隔空投送、接力
* iMessage、FaceTime
* 睡眠唤醒
* 独显硬件加速

##### 未测试功能

* Type-C接口（需要重新定制USBPorts.kext）



### 注意事项：

1. 采用定制USBPorts.kext，不一定可以通用，建议自己[定制](https://blog.daliansky.net/Intel-FB-Patcher-tutorial-and-insertion-pose.html#定制usb)一个
2. 使用随机生成的三码，建议使用Clover Configurator重新生成，以免与其他人的相同
3. 如果BCM943602cs是三天线，可能会影响2.4G WiFi和蓝牙同时使用（5G WiFi不受影响）



### 致谢

* [黑果小兵的部落阁](https://blog.daliansky.net)
