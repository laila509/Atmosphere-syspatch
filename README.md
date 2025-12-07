大气层1.10.0集成sys-patch插件破解包v6-莱莱踢个球
=====

2025.12.7，大气层1.10.0破解包v6发布，可以在1.10.0的v1-v5基础上覆盖升级，更新hekate_ctcaer_6.4.2_Nyx_1.8.2中文消除前一个版本部分型号主机开机卡logo的bug，更新DBI.nro-849英文版和849汉化版，更新JKSV.nro-12.02.2025中文。

2025.11.30，大气层1.10.0破解包v5发布，可以在1.10.0的v1-v4基础上覆盖升级，更新StatusMonitor.ovl-Zdm大佬终极汉化版消除bug，更新DBI.nro845英文版，更新极限超频sys-clk-EOS-1.7.0英文，loader.kip支持AMS1.10.0。更新CommonProblemResolver.bin，更新hekate中文的nyx.bin。

2025.11.27，大气层1.10.0破解包v4发布，可以在1.10.0的v1-v3基础上覆盖升级，StatusMonitor.ovl-1.3.2+英文消除Zdm大佬终极汉化版的取消bug，更新lockpick，更新DBI.nro844俄文版，Checkpoint.nro-3.10.2，NX-Activity-Log.nro-1.5.8中文，补充游戏安装器tinwoo。

2025.11.22，大气层1.10.0破解包v3发布，可以在1.10.0的v1v2基础上覆盖升级，更新DBI.nro-843汉化版和842俄文版，Goldleaf.nro，linkalho.nro，NX-Activity-Log.nro，wiliwili.nro，Tencent-switcher-GUI.nro，V3破解包除了极限超频loader.kip，其余插件和软件都兼容大气层1.10和SW21.0.0系统了。

2025.11.20，大气层1.10.0破解包v2发布，可以在1.10.0的v1基础上覆盖升级，更新sys-patch-158-5，更新Zdm大佬的汉化版ovlmenu-ultrahand，nx-ovlloader，ovl-sysmodules（国行系统如果升级20.0+会自动转全球系统），StatusMonitor和EdiZon，相册里更新Checkpoint.nro，DBI.nro-839俄文版，linkalho.nro-2.02英文，sphaira.nro-1.0.0中文兼容大气层1.10.0。所以除了极限超频loader.kip不可用（升级大气层文件记得删除TF卡上loader.kip和还原hekate_ipl.ini），相册里还剩Goldleaf.nro，NX-Activity-Log.nro，wiliwili.nro，DBI.nro-838汉化版还不兼容，建议相册nro用前端模式进，不会内存报错。虚拟系统如果联网内存报错启动飞行模式解决。

2025.11.18，大气层1.10.0破解包v1发布，更新atmosphere-1.10.0-prerelease-d9fc6e99e，hekate_ctcaer_6.4.1_Nyx_1.8.1，sys-patch_1.5.8-2，更新Lockpick_RCM.bin-1.9.16英文，万能前端hbmenu.nsp，更新全套Tesla插件为ppkantorski的英文版，当前的极限超频loader.kip不可用，Edizon金手指不可用。相册里更新JKSV.nro-11.16.2025中文，DeepseaToolbox.nro-47大佬汉化版，sphaira.nro-0.13.3中文（可以安装NSP），新增Awoo-Installer.nro-1.3.6中文，这些都支持大气层1.10.0。其余软件和插件都有兼容问题，只能等更新。

注意：
=====

（1）如果之前使用了linkalho假关联过任天堂账号，升级到21.0.0建议重新使用破解包里带mod版linkalho.nro重新假关联一次或者解除假关联，这样虚拟系统wifi下玩破解游戏会消除启动游戏弹窗的bug。但以后更新大气层文件还需要重新关联一次，所以最保险的还是解除账号关联或者启动飞行模式打开游戏。

（2）第一次使用集成sys-patch插件破解包需要看下面的更新TF卡大气层文件的说明，每次更新TF卡上的大气层文件，不能dbi.nro或者haze.nro来更新TF卡上的大气层破解包文件，建议选择1、重启hekate，在usb工具-SD卡这里usb数据线连win电脑。2、也可以选择关机取出TF卡，插入读卡器接win电脑。推荐每次SW系统大版本更新，比如19.0升级到20.0或21.0的时候，建议使用一键清理TF卡上旧的大气层破解包，再覆盖最新大气层破解包。

【一、什么是大气层集成sys-patch插件破解包】
=====

一直以来，大气层破解包就是基于大气层三件套：atmosphere，hekate，sigpatch三样核心组件，全SW破解机型通用。

hekate=SW主机的破解bootloader程序，用来加载atmosphere和sigpatch。

https://github.com/CTCaer/hekate/releases

atmosphere=用来破解SW官方系统权限，可以运行插件和软件。

https://github.com/Atmosphere-NX/Atmosphere/releases

sigpatch=外挂的大气层签名补丁，等大气层破解系统权限后玩各种破解游戏。

以上三件套缺一不可。但是由于atmosphere作者不支持玩破解游戏，自大气层1.7.0后阻止fusee.bin读取sigpatch外挂补丁中的fs和loader补丁，所以有大佬编译了atmosphere中的atmosphere/package3，stratosphere.romfs和bootloader/payloads/fusee.bin三个文件，把sigpatch内置，这样不需要外挂的大气层签名补丁。

sys-patch插件，是另一种以sysmodule启动插件的方式运行的大气层签名补丁，不像原来的sigpatch外挂，而是以插件形式，同时它的管理界面需要tesla-menu的ovl管理。那么你的TF卡上只要hekate+atmosphere，也能正常玩各种破解游戏。sys-patch每次系统启动都会自动加载，请确保TF卡上有atmosphere/contents/420000000000000B/flags/boot2.flag文件。等进入系统后就没事了，不用关闭也不用理它，自动生效的。

sys-patch插件其实就是允许玩破解游戏的工具，所以如果不让它启动，也不影响进入系统，操作其实就是删除atmosphere/contents/420000000000000B/flags/boot2.flag这个文件，但是所有的破解游戏或自制的NSP前端工具都无法运行，只能去deepsea工具箱后台打开它以后重启主机才能生效，才能玩破解游戏等。

sys-patch插件的发布者，sys-patch插件更新和其它sysmodule，ovl插件的更新是一样的，非常简单。

https://github.com/impeeza/sys-patch/releases

https://github.com/borntohonk/sys-patch/releases

整合大气层破解包这事儿本来就很普通，无脑的简单好弄，根本没有难度，莱莱不是什么大神大佬，只是搬运整合、总结分享大气层的相关文件，并无特意推广大气层破解包。所有大气层破解包不存在好坏，只是看个人使用习惯略有不同而已。破解包主要基于大气层三件套的组合，大家喜欢用就用，不喜欢用的也可以下论坛其他人发布的破解包或者干脆自己整合，因为所有的大气层破解包都可以根据需要进行编辑。

菜鸟都知道怎么整合大气层破解包

https://github.com/laila509/hekate_ipl

莱莱在原来奇乐融合大气层高级包的基础上，保留了基本的Tesla核心组件，edizon金手指和sys-clk超频，删除了其余多余的Tesla插件，确保系统稳定，但是也不妨碍大家自己添加。至于相册里的nro软件，那个并不太影响系统稳定，所以莱莱就保留了它们。

大气层集成sys-patch插件破解包因为插件少，几乎等于大气层纯净包，非常的稳定，不会出现报错，一般报错就是你的TF卡或者其它硬件问题。

<img src="https://github.com/laila509/QL-ATM-Package/blob/master/sys-patch-fileslist.jpg?raw=true" align="center" width="80%" />

<img src="https://github.com/laila509/QL-ATM-Package/blob/master/Atmosphere-1.7.1-v1-syspatch.jpg?raw=true" align="center" width="80%" />
