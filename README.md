# 微星B360M迫击炮-MOJAVE

作者：**Genius-lbesT**

**黑苹果Genius**

#### 关于微星B360M迫击炮:

![](https://github.com/Lubibest/MSI-B360M-MORTAR/blob/master/JPG/b360m-mortar-RGB.png)

| 芯片组   | Intel® B360 芯片组                                           |
| -------- | ------------------------------------------------------------ |
| 内存     | 4 条 DDR4 插槽，支持总合最高 64GB                            |
| 扩展插槽 | 2 个 PCIe 3.0 x16 插槽 (支持 x16/x4 模式) <br />2 个 PCIe 3.0 x1 插槽 |
| 板载显卡 | 1 个 DVI-D 接口，支持最高分辨率 1920x1200@60Hz <br />1 个 DisplayPort 接口 1.2，支持最高分辨率 4096X2304@60Hz <br />1 个 HDMI™ 接口 1.4，支持最高分辨率 4096x2160@30Hz |
| 存储     | 4 个 SATA 6Gb/s 接口 <br />2 个 M.2 插槽                     |
| 音效     | Dual Realtek® ALC892 解码芯片                                |
| 网络     | 1 x Intel I219-V Gigabit 网卡                                |
| 其他     | 微星B360M迫击炮在B360系列中拥有不俗的扩展性，<br />唯一的缺陷就是USB串口仅有一个，内置蓝牙的串口没地方插<br />解决方法：<br />某宝搜索：USB串口一分二 |



### 关于**迫击炮的BIOS**！！！

##### 1、关于微星B360M迫击炮的BIOS

经测试：

请在开始本教程前，使用[微星官网](https://cn.msi.com/Motherboard/support/B360M-MORTAR)下载微星B360M迫击炮**2018年5月24号**（7B23v12.zip）或**2018年8月2号**（7B23v13.zip）的BIOS或者本教程附件中的BIOS

刷入方法：将BIOS解压到U盘(FAT32格式)，使用M-FLASH刷入

将你的BIOS降级到这两个版本后，再进行本教程的操作

##### 2、使用最新版本的BIOS的朋友请在MAC的环境下，

用clover configurator添加RTC补丁

`Comment: Fix  RTC`

`Find: A00A9353 54415301`

`Replace: A00A910A FF0BFFFF`



# 正文

本教程将指导你安装最新版本的**MAC OS MOJAVE 10.14.5**

EFI支持：**10.14-10.14.5**  clover4928

支持安装的机器：

主板为**微星B360M迫击炮**的8/9代CPU的机器，

[下载本教程附件](https://github.com/Lubibest/MSI-B360M-MORTAR/archive/master.zip)

### 一、安装教程：

[How-to-install-a-Hackintosh](https://github.com/Lubibest/How-to-install-a-Hackintosh)

### 二、指南

##### 1、使用**EFI-FOR-NSTALL.ZIP**文件包中的**EFI文件**进行安装

##### 2、安装完成后，根据显卡的类别进行选择完善的EFI

---AMD显卡的使用**EFI-FOR-AFTER-INSTALL-AMD.ZIP**文件包中的**EFI文件**替换硬盘的**EFI分区**中的文件

---Intel核显的使用**EFI-FOR-AFTER-INSTALL-Intel.ZIP**文件包中的**EFI文件**替换硬盘的**EFI分区**中的文件

---Nvdia显卡的使用**EFI-FOR-AFTER-INSTALL-Nvdia.ZIP**文件包中的**EFI文件**替换硬盘的**EFI分区**中的文件

##### 3、然后进入系统

### 三、说明

##### 1、BIOS设置

进入BIOS首先重置一下BIOS设置

然后对一下选项进行操作：

`Super io  ->  disable`

`USB configurator -> XHCI Handoff-Enabled`

`CSM -> disable`

##### 2、已添加隐藏启动项：

显示启动项：四叶草界面按F3显示隐藏

- Recovery
- Preboot

### 四、USB端口定制设置

![]()

##### 1、使用**Hackintool**对端口进行定制：

![]()

##### 2、导出，桌面会生成4个文件

![]()

##### 3、将**USBPorts.kext**复制到EFI/CLOVER/KEXT/OTHER目录下

##### 4、将**USBInjectAll_v0.7.1.kext**删除

![]()

##### 5、完成定制

**注意事项**：更换机型之后，补丁将会失效

解决方法：将USBInjectAll_v0.7.1.kext放回EFI/CLOVER/KEXT/OTHER目录下

并在新机型下**重新定制**/或修改**USBPorts.kext**包内的**info.plist**为新设置的机型

### 五、本教程EFI

由

**垃圾帮主**修改制作

**Genius lbesT**发布

作者：**Genius-lbesT**

qq群：724096369

![](https://github.com/Lubibest/Hackintosh/blob/master/JPG/QQ.png)

 **黑苹果Genius**   [打赏](https://github.com/Lubibest/About-Genius-lbesT)

