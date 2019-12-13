### EFI概述

> 通过 [小兵](https://blog.daliansky.net/OpenCore-BootLoader.html) 和 [XJN](https://blog.xjn819.com/?p=543) 的博客，将 Clover引导[(点击跳转)](https://github.com/heyxiaobai/Asrock-Z370m-Pro4-Hackintosh/tree/clover-deprecated) 转换成 Opencore 引导

Mac 版本：10.15.2

Opencore 版本：0.5.3

更新日期：2019-12-13



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



### 你可能需要做的事

> 建议参考[小兵](https://blog.daliansky.net/OpenCore-BootLoader.html#deviceproperties-设备属性)、[XJN](https://blog.xjn819.com/?p=543)博客进行修改

1. [使用MacInfo](https://blog.daliansky.net/OpenCore-BootLoader.html#macserial)获取 或者 重新生成三码，以免与其他人的相同
2. 不同CPU可能需要设置电源管理（详见[XJN'S BLOG](https://blog.xjn819.com) 3.3～3.4）
3. 带核显的CPU[配置缓冲帧](https://blog.daliansky.net/OpenCore-BootLoader.html#deviceproperties-设备属性)
4. [定制](https://blog.daliansky.net/Intel-FB-Patcher-tutorial-and-insertion-pose.html#定制usb)USBPorts.kext



### 注意事项

1. 如果BCM943602cs是三天线，可能会影响2.4G WiFi和蓝牙同时使用（5G WiFi不受影响）



### 致谢

* [黑果小兵的部落阁](https://blog.daliansky.net)
* [XJN'S BLOG](https://blog.xjn819.com)
