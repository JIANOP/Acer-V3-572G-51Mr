## **三码入住（洗白）**

++注意事项++：

一：==非常重要==

共享efi，系统同序列号，可能导致==安全问题==，所以入住后==要分享==的efi都要==删除==序号以保证FaceTime，iMessage和Siri等等的正常使用

二：==重要==

如果以前登陆过，请网页登陆icloud删除设备----关闭网络---重启

导航到路径---你的用户名/Library/Preferences（图一）

查找并删除：

com.apple.iChat。

com.apple.icloud。

com.apple.ids.service

com.apple.imagent。

com.apple.imessage。

com.apple.imservice。

清空垃圾桶—重启

三：==必要条件==

点击桌面左上角苹果标志—关于本机—系统报告—点击左边“网络”确保有线网卡为en0（图二）
 
如果不是请内建网卡：

1、打开设置删除所有网络链接

2、打开finder，导航到/Library/Preferences/SystemConfiguration/（图三）

删除：NetworkInterfaces.plist和preferences.plist

清空垃圾桶---重启。

四：==准备入住==

1.在==clover==位置，使用==CloverConfigurator==打开==config.plist==配置文件

2.选择 ==**机型设置**== 在右边的“==双箭头==”（图四）选择匹配的型号（笔记本MacBook，台式iMac）

- 序列号验证附1

3.选择 ==**系统参数**== 自定义UUID 点击 **<从系统中获取>**（图五）

4.选择 ==**变量设置**== ->来自机型->生成（图六）

5.点击左上角苹果图标，打开-关于本机-系统报告-复制硬件UUID的序号（图七）

6.将复制的硬件UUID序号粘贴在 配置文件==机型设置 ->system ->SmUUID==（图八）

7.保存重启


---

附：

1.复制序列号到[EveryMac](https://everymac.com/ultimate-mac-lookup/)
来查找设备。如果序列号是正确，会出现机型配置，没有的话回去再点**序列号**==生成新的==，直到出现机型配置图（图九）

2.出现配置图后复制序列号到[苹果官网查看保障状态](https://checkcoverage.apple.com)：

如果出现==机型图==则不能用（说明Apple已经有这台电脑）（图十），回去==生成新的==序列号（按照附1重新查找）

如果出现红字 : ==很抱歉，这个序列号无效。请检查您的信息并再试一次。== （图十一）就可以用

