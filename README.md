大气层1.9.4集成sys-patch插件破解包v1-莱莱踢个球
====

大气层1.9.4最高支持20.4.0系统，向下兼容支持19.0等低版本系统。

2025.9.3，大气层1.9.4破解包v1发布，更新atmosphere-1.9.4-master-d7936d3fa，更新时鹏亮汉化版DBI806.nro，更新JKSV.nro-08.25.2025中文，极限超频sys-clk-EOS-1.6.7英文的loader.kip暂时不支持atmosphere-1.9.4，等更新loader.kip才能使用极限超频，之前使用极限超频的可以先删除改普通超频。


注意：
====

（1）莱莱从大气层1.9.1开始永久删除相册的一些无用且不怎么更新的NRO软件：Switch_90DNS_tester.nro、appstore.nro、Awoo-Installer.nro、ftpd.nro、nxdumptool.nro、NXThemesInstaller.nro（主题软件）、Haku33.nro、pplay.nro、switchtime.nro、tinfoil.nro。推荐使用一键清理TF卡上旧的大气层破解包文件v2。

（2）国行系统强制升级20.0.0+也不会变砖，其中zdm大佬开发的ovlmenu-ultrahand可自动将20.0.0+的国行系统转成国际系统。

（3）真实和虚拟在20.0.0+之后，如果想降级系统19.0.1或以下，需要在daybreak刷机、进系统前的维护模式做系统初始化，否则会报错。如果不降级系统就没事。。

第一次使用集成sys-patch插件破解包需要看下面的更新TF卡大气层文件的说明，只要你当前用的是莱莱发布的集成sys-patch插件大气层破解包，都是直接覆盖到TF卡完成大气层文件的更新升级，每次更新TF卡上的大气层文件，不能dbi.nro或者haze.nro，建议选（1）重启hekate，在usb工具-SD卡这里usb数据线连win电脑。（2）关机取出TF卡，插入读卡器接win电脑。如果你需要打开极限超频插件Switch-OC-Suite，每次大气层升级后也要覆盖一次，否则会被破解包中的普通超频插件替换。

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

<img src="https://github.com/laila509/QL-ATM-Package/blob/master/ATM-list1.jpg?raw=true" align="center" width="80%" />

<img src="https://github.com/laila509/QL-ATM-Package/blob/master/Atmosphere-1.7.1-v1-syspatch.jpg?raw=true" align="center" width="80%" />
