<img src="https://github.com/laila509/LeXiang-ATM/raw/master/LX-ATM.jpg" align="center" width="80%">

【分享】菜鸟都知道怎么整合大气层破解包

我不是什么大佬大神，也是和大家一样菜鸟入门，通过大佬大神们的教程，知道破解的流程，也学会整合大气层，通过使用觉得大气层越简单越好，那么多插件软件其实用途不大，而且可以根据需要增加。

【第一章，纯净包整合教程】

1.整合大气层首先做纯净包，就是Atmosphere+Hekate+Sigpatch的三件套，有了它就可以破解系统，运行已安装的破解游戏。纯净包是基础包可直接用，只要加合适的引导就可适用所有破解机，不区分软破用的TX注入器或DQC注入器，不区分TX芯片还是HW芯片，软硬破通用。

大气层整合包=纯净包+搭配包，搭配包就是特斯拉等一众插件和相册NRO软件的组合，搭配包不能直接使用，需要覆盖到纯净包或其它大气层整合包上使用，整合包应实用为主，需要插件和软件多少可以不断的添加删减。

2.最新的三件套版本是Atmosphere1.3.2，Hekate5.7.2，Sigpatchfor14.1.0/14.1.1

Atmosphere，https://github.com/Atmosphere-NX/Atmosphere/releases

下atmosphere-1.3.2-master-e96972c93+hbl-2.4.1+hbmenu-3.5.0.zip和fusee.bin，解包后是[atmosphere],[switch]和hbmenu.nro

Hekate，https://github.com/CTCaer/hekate/releases

下hekate_ctcaer_5.7.2_Nyx_1.2.2.zip，解包后是[bootloader]和hekate_ctcaer_5.7.2.bin

Sigpatch，https://github.com/ITotalJustice/patches/releases

下Sigpatches.zip，解包后是[atmosphere]和[Bootloader

3.三件套不分先后复制到同一目录，fusee.bin移至/bootloader/payloads/

4.通用的大气层设置，适用所有大气层包，在乐享或奇想大气层纯净包中找

override_config.ini，stratosphere.ini和system_settings.ini复制/atmosphere/config/

exosphere.ini，万能前端hbmenu.nsp和sx gear的boot.dat复制根目录

把hekate_ctcaer_5.7.2.bin重命名payload.bin

把Lockpick_RCM.bin，TegraExplorer.bin等常用引导文件复制/bootloader/payloads/

emummc.txt复制/atmosphere/hosts/

如想真实破解系统也开hosts和序号保护，把emummc.txt再复制成sysmmc.txt，打开exosphere.ini把blank_prodinfo_sysmmc=0改成blank_prodinfo_sysmmc=1保存。

5.自编的Hekate设置，所有大气层包就这差别，可参照乐享或奇想大气层包调整

/bootloader/hekate_ipl.ini是启动文件，设置启动全靠它

/bootloader/bootlogo.bmp是开机图，720×1280，32位，文件名和位置以hekate_ipl.ini为准

/bootloader/res/的图片是开机图标，文件名和位置以hekate_ipl.ini

/bootloader/ini/的启动文件也和hekate_ipl.ini相似，在launch右边的more configs出现

6.后期升级三件套，只要在原版本上对比添加新的组件就行了

下Beyond Compare，左右两边分别是旧整合包和新的三件套组件，区分哪些需要更新
