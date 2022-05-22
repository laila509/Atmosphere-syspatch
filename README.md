【分享】菜鸟都知道怎么整合大气层破解包

我不是什么大佬大神，也是和大家一样菜鸟入门，通过大佬大神们的教程，知道破解的流程，也学会整合大气层，通过使用觉得大气层越简单越好，那么多插件软件其实用途不大，而且可以根据需要增加。

【第一章，大气层纯净包整合教程】

1.整合大气层首先做纯净包，就是Atmosphere+Hekate+Sigpatch的三件套，有了它就可以破解系统，运行已安装的破解游戏。纯净包是基础包可直接用，只要加合适的引导就可适用所有破解机，不区分软破用的TX注入器或DQC注入器，不区分TX芯片还是HW芯片，软硬破通用。
    
大气层整合包=纯净包+搭配包，搭配包就是特斯拉等一众插件和相册NRO软件的组合，搭配包不能直接使用，需要覆盖到纯净包或其它大气层整合包上使用，整合包应实用为主，需要插件和软件多少可以不断的添加删减。
    
2.最新的三件套版本是Atmosphere1.3.2，Hekate5.7.2，Sigpatchfor14.1.0/14.1.1
    
Atmosphere，https://github.com/Atmosphere-NX/Atmosphere/releases
    
下atmosphere-1.3.2-master-e96972c93+hbl-2.4.1+hbmenu-3.5.0.zip和fusee.bin，解包后是[atmosphere],[switch]和hbmenu.nro
    
Hekate，https://github.com/CTCaer/hekate/releases
    
下hekate_ctcaer_5.7.2_Nyx_1.2.2.zip，解包后是[bootloader]和hekate_ctcaer_5.7.2.bin
    
Sigpatch，https://github.com/ITotalJustice/patches/releases
    
下Sigpatches.zip，解包后是[atmosphere]和[Bootloader]
    
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

/bootloader/bootlogo.bmp是开机图，文件名和位置以hekate_ipl.ini为准

/bootloader/res/的图片是启动图标，文件名和位置以hekate_ipl.ini为准

/bootloader/ini/的启动文件也和hekate_ipl.ini相似，在launch右边的more configs出现

6.后期升级三件套，只要在原版本上对比添加新的组件就行了
    
下Beyond Compare，左右两边分别是旧整合包和新的三件套组件，区分哪些需要更新

【第二章，大气层纯净包文件列表】

[atmosphere]，是大气层的核心

  --[config]，大气层配置文件
  
    --override_config.ini，非必要，大气层默认设置
    
    --stratosphere.ini，非必要，Hekate设置autonogc=1也可以
    
    --system_settings.ini，必要，开hosts和关闭金手指自动启动
    
  --[exefs_patches]，大气层插件
  
     --[es_patches]，es插件，与SW系统对应，因大气层向下兼容，所以所有SW系统都放上
     
        --这里一堆IPS文件，如现在总共有22个IPS文件，其中一个对应14.1.0/14.1.1系统
        
     --[nfim_ctest]，免联服务器插件，与SW系统对应，同样都放上
     
        --这里一堆IPS文件，和es插件同理
        
  --[fatal_errors]，非必要，大气层运行出错会生成日志
  
  --[flags]，非必要，可删
  
  --[hbl_html]，非必要，可删
  
  --[hosts]，host列表保护，阻止连服务器
  
    --default.txt，默认不用管
    
    --emummc.txt，这是在虚拟系统做host保护
    
  --[kip_patches]，大气层插件
  
    --[fs_patches]，fs插件，和es插件同理
    
        --这里一堆IPS文件，但每次更新fs插件是2个，分别是exfat和fat
        
    --[loader_patches]，loader插件，与大气层版本对应，只需要一个
    
        --这里只需一个IPS文件，对应大气层版本，就是与当前package3对应
        
  --hbl.nsp，有了它才能进相册，homebrew启动器
  
  --package3，大气层模块，以前名叫fusee-secondary.bin
  
  --reboot_payload.bin，重启payload，可以在Hekate设置，也可以用Hekate重命名
  
  --stratosphere.romfs，大气层模块，和package3，fusee.bin构成大气层基本核心
  
[bootloader]，是Hekate的核心

  --[ini]，是Hekate中more configs的引导配置
  
    --lakka.ini，非必要，可以编辑
    
  --[payloads]，可以在Hekate中加载它们
  
    --commonproblemresolver.bin，一键关闭插件启动和删除主题，解决开机问题
    
    --fusee.bin，大气层原版引导模块
    
    --lockpick_rcm.bin，主机Keys获取工具
    
    --tegraexplorer.bin，主机固件获取工具
    
  --[res]，Hekate的图标、开机图等，可以编辑，需Hekate_ipl.ini调整
  
    --图标分辨率192*192，开机图720*1280，位深度都是32
    
    --[sys]，Hekate模块，和Hekate.bin构成Hekate基本核心
    
    --这里几个文件都是必要的
    
  --bootlogo.bmp，开机图，
  
  --hekate_ipl.ini，Hekate启动设置文件
  
  --patches.ini，fss0引导的FS和Loader插件以文本，和fusee引导不一样
  
  --update.bin，最新Hekate.bin的重命名，不需要更新注入器的Payload.bin
  
[switch]，所有相册的NRO软件，特斯拉的OVL插件都在这里

  --daybreak.nro，大气层用Daybreak离线升级系统
  
boot.dat，它如果是SX Gear的boot文件，TX注入器或TX芯片转大气层必要

exosphere.ini，大气层配置文件，设置虚拟系统隐藏序号保护

hbmenu.nro，相册的工具菜单

hbmenu.nsp，万能前端，相册的工具菜单有高权限

payload.bin，硬破机需要它来启动，TX转大气层也是启动它





