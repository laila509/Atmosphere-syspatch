大气层1.11.0集成sys-patch插件破解包v0beta-莱莱踢个球
=====

大气层1.11.0最高支持22.0.0系统，向下兼容支持21.x、19.x等低版本系统，可以在莱莱之前发的破解包1.10.0/1.10.1/1.10.2/1.10.3的基础上覆盖升级。

2026.3.23，大气层1.11.0破解包v0beta发布，更新lsp编译的atmosphere1.11.0测试版（替换package3和stratosphere.romfs两个文件，屏蔽hekate_ipl.ini中的ATM-Auto：大气层自动选择的加载选项，等正式版大气层1.11.0的fusee.bin更新再恢复）。重命名sphaira.nro替换根目录的hbmenu.nro，进相册就是sphaira菜单，主要为了方便虚拟系统下进相册新建daybreak前端桌面图标，支持22.0.0降级21.2.0后使用虚拟系统，毕竟22.0.0虚拟系统玩破解游戏偶尔会出现sys-ptach失效导致游戏无法运行，需要重启解决。真实系统安装前端会被BAN机，建议新机入手升级22.0.0正版系统后再破解的就不要再去动22.0.0真实系统了。

注意：
=====

（1）目前SW22.0.0系统下的hbmenu所有nro软件只能以前端游戏方式打开运行不报错（不是hbmenu的万能前端），真实系统安装前端会导致ban机，所以建议新机破解后已经联网升级22.0.0的，首先新建22.0.0的虚拟系统，再进虚拟22系统通过相册sphaira.nro菜单，移动光标到daybreak，按X键新建前端，然后返回主菜单，运行daybreak，降级刷到21.2.0，重启后21.2.0的所有相册nro软件均可直接运行，也可以通过万能前端运行nro软件，不会再报错。如果坚持22.0.0虚拟系统的，建议对DBI，JKSV安装前端，这样也满足日常需要了，如果觉得桌面软件图标太多影响点击游戏图标，可以每次安装一个用完就删，需要的时候再去安装，在虚拟系统里折腾没事儿。

（2）现在Zdm大佬终极汉化版的Tesla-ultrahand插件，开机启动会识别20.0+的国行系统自动转成全球系统，国行升级20.0+不会再变砖，也不再需要手动tencent-switcher-gui.nro或者Tesla的ovl-sysmodules.ovl去做系统一键转区。大气层破解包更新了system_setting的配置，所以虚拟系统wifi下玩破解游戏可以自动消除启动游戏弹窗的bug。

（3）第一次使用集成sys-patch插件破解包需要看下面的更新TF卡大气层文件的说明，每次更新TF卡上的大气层文件，不能dbi.nro或者haze.nro来更新TF卡上的大气层破解包文件，建议选择1、重启hekate，在usb工具-SD卡这里usb数据线连win电脑。2、也可以选择关机取出TF卡，插入读卡器接win电脑。推荐每次SW系统大版本更新，比如19.0升级到20.0或21.0的时候，建议使用一键清理TF卡上旧的大气层破解包，再覆盖最新大气层破解包。

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
