# MSI/B360MOTOR/Hackintosh

关于我发布的EFI，您需要知道：

## 在您使用此EFI后，记得使用OpenCore Configurator刷写三码！

## 配置信息：

我的配置是根据黑苹果较为完善的进行选取搭配
| Hackintosh | 配置单 |
|---|---|
|  CPU | Intel i3 9100F（理论上所有8、9代CPU即coffee lake架构都可使用） |
|---|---|
|  GPU | 蓝宝石 Radeon RX580 4G |
|  主板 | MSI B360 MOTOR（B360芯片组） |
|  内存 | CUSO 2666Mhz 8G X2 |
|  机型 | iMac Pro 2017 |
| 无线网卡 | 博通94360CD 双频四天线|

## 非正常工作

* 麦克风（我未外置购买麦克风，无法测试）
* 随航（我的CPU不带有核显，无法使用）
* 如有更多需要，你可以进行反馈和联系我。

## Bios 设置
* Advanced • CPU Configuration • CFG Lock = Disabled
* Advanced • Chipset Configuration • Above 4G Decoding = Disabled | or Enabled
* Advanced • Chipset Configuration • IGPU Multi-Monitor = Disabled
* Advanced • USB Configuration • XHCI Hand-off = Enabled
* Security • Secure Boot = Disabled

## 截图预览
<img width="2048" alt="截屏2021-10-03 下午10 30 44" src="https://user-images.githubusercontent.com/91834755/135758508-ba9a702d-cb60-4a76-a186-fae062530f88.png">


## 更新日志

v1.0 2021.10.03
* OC引导版本为0.7.4
* 解决了“Boot Install macOS xxxx"的启动项不显示问题
* 机型为iMac Pro
* 精简不必要的开机启动项，默认添加“Reset NVRAM“以及”SIP 状态一键切换“（需点击空格唤出）
* 当您使用OpenCore Configurator工具刷写三码后即可正常使用iMessages以及Facetime

v2.0.x 2021.10.17-10.26
* OC版本为0.7.4官方发行版
* 修复无法安装Catalina及以下版本的问题
* 添加支持macOS Monterey 12.0.1 (21A559)支持
* 修复无法从系统更新中获取更新的错误

