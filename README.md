大气层1.8.0集成sys-patch插件破解包
=====

2025.3.27，大气层1.8.0破解包v15发布，更新Checkpoint.nro-3.8.1英文（依然需要前端模式运行该软件），DBI.nro-775俄文。

2025.2.27，大气层1.8.0破解包v14发布，更新DBI.nro-763俄文，wiliwili.nro-1.5.1中文，更新“一键清理TF卡上旧的大气层破解包文件v2”，可删除旧的破解包文件。

2025.2.2，大气层1.8.0破解包v13发布，更新DBI.nro-750俄文，nxdumptool.nro，更新极限超频插件EOS1.5.1，新加“一键清理TF卡上旧的大气层破解包文件”，可删除旧的破解包文件。

2025.1.6，大气层1.8.0破解包v12发布，更新DBI.nro-749俄文，新加tinwoo.nro-1.0.27（类Awoo）

2024.12.11，大气层1.8.0破解包v11发布，更新sys-patch-156，Tinfoil.nro-19.0v1前端版中文，ovlsysmodule中文。

2024.11.30，大气层1.8.0破解包v10发布，更新最新英文原版Tesla-ultrahand全套插件，包括edizon金手指和sys-clk超频插件，更新NX-Activity-Log.nro-1.5.4中文，新加最新俄文版dbi731，路径在switch/dbi-ru/。删除AtmoXL-Titel-Installer.nro，Calculator_NX.nro，Firmware-Dumper.nro，NX-Shell.nro四个基本废弃的nro软件，所以不影响覆盖升级，都在switch/文件夹下。

2024.11.18，大气层1.8.0破解包v9发布，更新sys-patch-155英文，更新NX-Activity-Log.nro-1.5.2中文，ftpd.nro-3.2.1英文。

2024.11.10，大气层1.8.0破解包v8发布，更新zdm大佬编译的nyx.bin修复文件，编译的全套Tesla插件，更新NX-Activity-Log.nro-1.5.1中文。

2024.11.6，大气层1.8.0破解包v7发布，换回v4的easyworld编译汉化Hekate的nyx.bin文件，更新JKSV.nro-11.05.2024，linkalho.nro，nxdumptool.nro。

2024.10.27，大气层1.8.0破解包v6发布，更新sys-patch-154，修复了17.0.0系统的bug，虽然玩大气层的都知道只要大气层更新最高支持19.0.0系统，那就没人会降级到17.0.0或更低的，肯定daybreak刷系统到19.0.0或18.1.0。

2024.10.25，大气层1.8.0破解包v5发布，更新zdm大佬编译的汉化版hekate，中英文版的ovlloader，ovlmenu-ultrahand，sys-clk.ovl，StatusMonitor.ovl，EdiZon，ovlsysmodule，NX-Activity-Log.nro和NX-Shell.nro，更新wiliwili.nro-1.5.0，更新sys-patch_153_forwarders_2。

2024.10.20，大气层1.8.0破解包v4发布，更新ovlloader-1.0.9+，ovlmenu-ultrahand-1.7.9中文。

2024.10.17，大气层1.8.0破解包v3发布，更新atmosphere-1.8.0-prerelease-c6014b533（sys-patch-1.5.2-fw19继续支持，无需更新），更新sys-clk.ovl-2.0.1英文、更新极限超频插件EOS1.5.0支持大气层1.8.0。

2024.10.14晚，大气层1.8.0破解包v2发布，和1.8.0破解包v1一样，如有极限超频EOS的，要先删loader.kip后再覆盖完成升级。更新主题补丁theme-patches最高支持19.0.0，themes/systemPatches18.1.0/是主题补丁的备份，也是支持19.0.0的，不修改文件夹名称为了方便大气层破解包的覆盖升级。更新nxdumptool.nro，替换tinfoil.nro为applet版的nro，和wiliwili.nro一样，通过安装新的万能前端hbmenu或按住R进游戏的方式打开相册里的nro软件。

2024.10.14，大气层1.8.0破解包v1发布，更新atmosphere-1.8.0-preprerelease-5717ea6c0，hekate_ctcaer_6.2.2_Nyx_1.6.4中文，sys-patch-1.5.2-fw19，最高支持SW19.0.0系统，可以玩破解游戏了。更新Lockpick_RCM.bin-1.9.13英文，StatusMonitor.ovl-1.1.4英文，sys-clk.ovl-2.0.0-dev1900-poc英文，新的万能前端hbmenu.nsp，需删除桌面旧的hbmenu图标后再安装，否则会有两个hbmenu。

第一次使用集成sys-patch插件破解包需要看下面的更新TF卡大气层文件的说明，只要你当前用的是莱莱发布的集成sys-patch插件大气层破解包，更新日志里没有特别说明，以后都是直接覆盖到TF卡完成大气层文件的更新升级，极限超频插件每次升级后也要覆盖一次，否则会被破解包中的普通超频插件替换。

【一、什么是大气层集成sys-patch插件破解包】

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
