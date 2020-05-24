

# 华擎玩家至尊Z370 Gaming-ITX/ac，10.15.4，opencore0.5.8引导EFI文件

​       本来想用人家的配置，谁知道不能直接套用，主板明明一样，无奈只能自己配置config，更新opencore版本为0.5.8

更新底包驱动为最新版,没问题的话暂时不更新了

## BIOS设置

CFG Lock    禁用

Intel 虚拟化技术    >>开启

SGX     >>禁用

4G Decoding    >>启用

VT-d    >>禁用

IOAPIC 24-119 Entries     >>关闭

IGPU 多监视器      >> 开启

XHCI Hand-off        >>开启

Intel（R） Platform Trust Technology     >>禁用

快速启动   >>关闭

CSM     >>关闭

## 主机配置：

主板：Fatal1ty-Z370-Gaming-ITX-ac

CPU：intel core i5 9400         	    后续会升级，只为亮机，毕竟家境贫寒

显卡：迪兰RX 470 4G X-Serial   	免驱动，刷了技嘉RX570的vbios，解决UEFI花屏问题

声卡：Realtek ALC1220   		      注入alcid=11

内存：科赋CJR2666  				     16GBx2

无线网卡蓝牙：BCM943602CS  原生免驱，需要购买。替换自带无线网卡即可

## 截图：

目前SMBIOS选择为iMac 19,2 ,CPU如果是i9 可以改为iMac 19,1

**关于本机**

<img src="https://emiya.oss-cn-shanghai.aliyuncs.com/%E5%85%B3%E4%BA%8E%E6%9C%AC%E6%9C%BA9400.png" style="zoom:67%;" />

**集显，用作运算，剪辑神助攻**

![](https://emiya.oss-cn-shanghai.aliyuncs.com/%E9%9B%86%E6%98%BE630.png)

**显卡，刷成RX570**

<img src="https://emiya.oss-cn-shanghai.aliyuncs.com/470%E6%98%BE%E5%8D%A1.png" style="zoom: 67%;" />

**WiFi蓝牙**

![](https://emiya.oss-cn-shanghai.aliyuncs.com/WiFi%E8%93%9D%E7%89%99.png)

**音频ALC1220，注入alc_id为11**

<img src="https://emiya.oss-cn-shanghai.aliyuncs.com/z370%E9%9F%B3%E9%A2%91.png" style="zoom:67%;" /> 



**参考EFI:** 

https://github.com/fangf2018/ASRock-Z370-Fatal1ty-ITX-Clover-hackintosh

https://github.com/fangf2018/ASRock-Z370-Fatal1ty-ITX-OpenCore-hackintosh