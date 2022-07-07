# MSI B360m Hackintosh EFI

关于我发布的EFI，您需要知道：

## ❗️在您使用此EFI后，记得使用OpenCore Configurator刷写三码！
## ❗️所有操作都在您可控范围内执行，若出现错误及任何软硬件损坏本人概不负责！

## 配置信息：

我的配置是根据黑苹果较为完善的进行选取搭配
| Hackintosh | 配置单 |
|---|---|
|  CPU | Intel i3 9100F（理论上所有8、9代CPU即coffee lake架构都可使用） |
|  GPU | SAPPHIRE Radeon RX580 4G |
|  主板 | MSI B360 MOTOR（B360芯片组） |
|  内存 | CUSO 2666Mhz 8G X2 |
|  机型 | iMac Pro 2017 |
| Wifi | Broadcom 94360CD|

## No Working ❌

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
<img width="2048" alt="截屏2022-06-20 14 05 02" src="https://user-images.githubusercontent.com/91834755/174536899-1b263bb4-19b5-4b79-9cbc-6099d94d5125.png">



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

v2.0.2 2022.06.19-06.20
* OC引导更新为0.8.2PrePublic
* 添加支持macOS Ventura 13.0（22A5266r）支持
* 修复部分错误

v3.0 2022.07.07
* OC引导更新为0.8.3Beta
* 修复macOS 13 Beta3 更新问题
* 更新Lilu.kext
* 恢复"Reset NVRAM"以及“SIP状态切换"
