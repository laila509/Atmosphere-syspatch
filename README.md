大气层1.9.1集成sys-patch插件破解包
=====

大气层1.9.1最高支持20.1.0系统

2025.5.29，大气层1.9.1破解包v1发布，更新atmosphere-1.9.1-master-b11850b3a+hbl-2.4.4+hbmenu-3.6.0，hekate_ctcaer_6.3.1_Nyx_1.7.0中文，sys-patch继续有效，更新ovlmenu-ultrahand-1.8.5中文，StatusMonitor.ovl-1.1.9英文。因为删除部分相册里不太常用的NRO软件，破解包体积大幅缩小。建议此次更新先使用【一键清理TF卡上旧的大气层破解包文件v2】后再覆盖，或者自行在TF：switch/删除相应的文件夹和NRO文件，注意原来tinfoil自动生成前端的，最好删除桌面主页上tinfoil的大图标，否则还要再去删除TF：switch/tinfoil的目录。普通超频有效，极限超频的loader.kip暂时未支持，建议暂时删除TF：atmosphere/kips/loader.kip。

注意：
=====

（1）莱莱从大气层1.9.1开始永久删除相册的一些无用且不怎么更新的NRO软件：Switch_90DNS_tester.nro、appstore.nro、Awoo-Installer.nro、ftpd.nro、nxdumptool.nro、NXThemesInstaller.nro（主题软件）、Haku33.nro、pplay.nro、switchtime.nro、tinfoil.nro。

（2）国行系统不可直接升级20.0.0+，强刷升级的绝对变砖，必须在19.0.1或以下的系统里先通过tencent-switcher-gui.nro或者Tesla的ovl-sysmodules.ovl，一键转成全球系统，才可以刷机升级20.0.0+。转成全球系统的20.0.0+也绝对不可以通过软件转回国行系统！慎！

（3）真实和虚拟在20.0.0+之后，如果想降级系统19.0.1或以下，需要在daybreak刷机、进系统前的维护模式做系统初始化，否则会报错。如果不降级系统就没事。如果遇到开启wifi后待机的耗电异常高，可以开启飞行模式解决问题。

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
