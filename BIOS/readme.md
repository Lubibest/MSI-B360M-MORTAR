### 关于**迫击炮的BIOS**！！！

#### 1、关于微星B360M迫击炮的BIOS

请在开始本教程前，在[微星官网](https://cn.msi.com/Motherboard/support/B360M-MORTAR)下载或者本教程附件中微星B360M迫击炮**2018年5月24号**（7B23v12.zip）或**2018年8月2号**（7B23v13.zip）的BIOS，刷入BIOS

刷入方法：将BIOS解压到U盘(FAT32格式)，插入USB2.0端口，在BIOS界面使用M-FLASH刷入

将你的BIOS降级到这两个版本后，再进行本教程的操作

#### 2、如果想用最新版本BIOS的朋友请在MAC的环境下，

用clover configurator添加RTC补丁

`Comment: Fix  RTC`

`Find: A00A9353 54415301`

`Replace: A00A910A FF0BFFFF`
