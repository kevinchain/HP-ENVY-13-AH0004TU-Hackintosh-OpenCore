# HP-ENVY-13-AH0004TU-Hackintosh-OpenCore

[本文地址](https://github.com/ongengi/HP-ENVY-13-AH0004TU-Hackintosh-OpenCore)

## 更新日志

- 2020-06-10

  使用 [Dennis Koluris](https://github.com/chris1111) 的 [EFI](https://github.com/dkoluris/HP-ENVY-13-AH0002-OpenCore) 重构 ACPI 

- 2020-05-19

  从 Clover 迁移 至 OpenCore

- 2020-05-15

  内建网卡，解决 App Store 登录验证，感谢 [亦蔚然](https://www.zhihu.com/people/leo_logic) 提供的网卡内建方法


## 硬件配置

|   配件   |             规格              | 工作状态 |
| :------: | :---------------------------: | :------: |
|   型号   |      HP-ENVY-13-AH0004TU      |     √     |
|  处理器  |     Intel® Core™ i5-8250U     |     √     |
|   内存   |    8GB Dual LPDDR3 2133Mhz    |     √     |
|   硬盘   |      LITEON CA1-8D256-HP      |     √     |
| 核芯显卡 |   Intel(R) UHD Graphics 620   |     √     |
|   声卡   |        Realtek ALC285         |     √     |
| 无线网卡 |    ~~Intel Wireless-AC 7265~~ / ASUS USB-AC53 Nano     |     √     |
|  显示器  |  LGD0597 13.3" IPS 1920x1080  |     √     |

## BIOS

BIOS 版本号 为 F.25 Rev.A

BIOS 设置为 默认，关闭 Secure Boot（安全启动）

## 重要

- 注入新的 **三码**

- 不使用 **文件保险箱（FileVault）**

- 关闭 **软件更新**

- 在 `系统偏好设置` -> `节能` 选项卡中，取消 `小憩` 和 `唤醒以供Wi-Fi网络访问` 的勾选

- 在 `系统偏好设置` -> `蓝牙` -> `高级` 选项卡中，取消所有勾选

## 问题

- USB、摄像头、蓝牙 未定制
- ~~FaceTime、iMassage 不可用~~
- ~~Siri 可触发，但是无论说什么都提示 *“请复读一遍”*~~

- ~~App Store 无限登录~~

## 硬件驱动状况

### 1. 显示

使用 [one-key-hidpi](https://github.com/xzhih/one-key-hidpi) 项目开启 **HiDPI**，以防止瞎眼

### 2. CPU变频

正常

### 3. 屏幕背光

正常，可使用组合键 Fn+F3、Fn+F4 调节

### 4. SD 读卡器

GG

### 5. 扬声器

使用 Hackintool 仿冒声卡，并注入 id 11，驱动 C 面两个扬声器

### 6. 无线网卡

使用 USB无线网卡 ASUS USB-AC53 Nano

官网驱动仅支持至 Catalina 10.13，遂使用 [Wireless-USB-Adapter](https://github.com/chris1111/Wireless-USB-Adapter)

使用正常

### 7. USB、蓝牙、摄像头

正常，使用 USBInjectAll 驱动

### 8. SSD

正常

### 9. SMC

正常

### 10. 电池

正常

### 11. 触控板

正常

## 特别感谢

感谢各位大佬的教程和帮助

[Dennis Koluris](https://github.com/dkoluris)

[墨色之银](https://github.com/SilentSliver)

[醉啦]()

[亦蔚然](https://www.zhihu.com/people/leo_logic)

[大头蔡Cass](https://space.bilibili.com/16323318/)

[独行秀才的老窝](https://shuiyunxc.gitee.io/)

[Sukka's Blog](https://blog.skk.moe/) 

[Xjn's Blog](https://blog.xjn819.com/)

[黑果小兵的部落阁](https://blog.daliansky.net/)

