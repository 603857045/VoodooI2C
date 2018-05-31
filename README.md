![release](https://img.shields.io/github/release/alexandred/VoodooI2C.svg) ![circleci](https://circleci.com/gh/alexandred/VoodooI2C.svg?style=shield&circle-token=:circle-token) [![Gitter chat](https://img.shields.io/gitter/room/nwjs/nw.js.svg?colorB=ed1965)](https://gitter.im/alexandred/VoodooI2C)

## 什么是VoodooI2C？
VoodooI2C是一个由macOS内核扩展组成的项目，增加了对I2C总线设备的支持。该项目分为两个主要组成部分：核心扩展和各种其他卫星扩展。

## 核心
核心是VoodooI2C.kext内核扩展。此kext旨在由计算机需要某种形式的I2C支持的任何人安装。它由I2C控制器驱动程序组成，负责将设备结点发布到IOService平面。

## 卫星
卫星是各种内核扩展的集合，支持特定类型的I2C器件。卫星kext的一个例子是VoodooI2CHID.kext增加了对I2C-HID设备的支持。通常，用户将为每类I2C器件安装一个卫星kext。

## 当前状态
以下英特尔I2C控制器完全受支持：

INT33C2和INT33C3- 哈斯韦尔时代
INT3432和INT3433- 布罗德威尔时代
pci8086,9d60，pci8086,9d61，pci8086,a160和pci8086,a161- SKYLAKE微架构/ Kabylake时代
以下设备类完全支持：

I2C-HID设备
ELAN设备
请注意，设备类之间有时会有重叠。例如，一些ELAN设备也可能是I2C-HID设备。

## 发布
最新版本是发布，可以在发布页面上下载。

## 兼容性
请检查VoodooI2C wiki上的兼容性页面，以确定您的设备是否兼容。如果它不在列表中，但您仍然怀疑VoodooI2C可能适合您，请通过我们的Gitter页面与我们联系。

## 文档和故障排除
请访问文档站点以获取有关如何安装和排除VoodooI2C故障的更多信息。

## 执照
该程序受GPL许可证保护。请参阅该LICENSE.txt文件以获取更多信息

## 特约
我们正在寻找能够胜任的C ++，OS X内核，Linux内核，I2C，HID等开发人员来帮助改进此项目！以下是贡献的指导原则：

将此存储库分叉并克隆到本地计算机
创建一个新的功能分支并添加提交
将你的功能分支推到你的叉子上
向上游提交拉取请求
## 捐赠
可以通过比特币捐赠给以下钱包：https：//live.blockcypher.com/btc/address/1EUxSExh8XCveWxVDVQqnez2o95AnG8Qhr/。
