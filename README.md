

# 华擎玩家至尊Z370 Gaming-ITX/ac，10.15.4，opencore0.5.8引导EFI文件

​       本来想用人家的配置，谁知道不能直接套用，主板明明一样，无奈只能自己配置config，更新opencore版本为0.5.8

更新底包驱动为最新版,没问题的话暂时不更新了

## BIOS设置

bios版本为410，为了改开机第一屏为苹果logo，本着抄作业要完美的原则，要刷的话直接可以开车，bios可以随意升降级，只要不断电，都好说

CFG Lock    禁用

Intel 虚拟化技术    >>开启

SGX     >>禁用

4G Decoding    >>启用

VT-d    >>禁用

IOAPIC 24-119 Entries     >>关闭

IGPU 多监视器      >> 开启

共享显存    >>128M

XHCI Hand-off        >>开启

Intel（R） Platform Trust Technology     >>禁用

快速启动   >>关闭

CSM     >>关闭

## 主机配置：

主板：Fatal1ty-Z370-Gaming-ITX-ac

CPU：intel core i5 9400         	    后续会升级，只为亮机，毕竟家境贫寒

显卡：迪兰RX 470 4G X-Serial   	免驱动，刷了技嘉RX570的vbios，解决UEFI花屏问题，强迫症

声卡：Realtek ALC1220   		      注入alcid=11

内存：科赋CJR2666  				     16GBx2

无线网卡蓝牙：BCM943602CS  原生免驱，需要购买。替换自带无线网卡即可

## 截图：

目前SMBIOS选择为iMac 19,2 ,CPU如果是i9 可以改为iMac 19,1

**关于本机**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/关于本机9400.png)

**集显，用作运算，剪辑神助攻**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/集显630.png)

**显卡，刷成RX570**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/470显卡.png)

**WiFi蓝牙**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/WiFi蓝牙.png)

**音频ALC1220，注入alc_id为11**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/z370音频.png) 

**UEFI花屏**

![](https://cdn.jsdelivr.net/gh/MikasaEmiya/images/img/UEFI花屏.jpg)

**解决方案：**

目前只能强刷RX570的VBIOS，同品牌的RX570频率，内存颗粒都不同，不敢开车，只能刷技嘉的了，提供原版vbios

和技嘉vbios，刷bios有风险，请科学开车，不提供刷bios教程，自行百度

**参考EFI:** 

https://github.com/fangf2018/ASRock-Z370-Fatal1ty-ITX-Clover-hackintosh

https://github.com/fangf2018/ASRock-Z370-Fatal1ty-ITX-OpenCore-hackintosh