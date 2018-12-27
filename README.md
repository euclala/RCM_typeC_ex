#**RCM-X86 type-C usb dongle**  

* * *

# Normally please use the /V3   UF2 files to flash the dongle

There are three version dongle : V1pcb, V2ex,V3), most of the dongle version is V3.

Another dongle PCB chip->[internal_Dongle](https://github.com/euclala/RCM-X86/tree/master/internalDongle)

* * *

## UF2 file introduction (UF2文件说明)
 hekate_ctcaer-> hekate-ctcaer(大气层)  
 TXOS -> TEAM xecuter os 1.0 (OS系统)  
 reiNX -> ReiNX  
 SDpayload -> payload from SD card  
  
## Directory introduction (目录介绍)
  \internalDongle  Solder inside dongle 内置嵌入式注入器  
  \V1pcb   PCB version 超级电容,黑色PCB电路板版本  
  \V2ex      V2 version (before 2018-08-01)使用电池的版本2018年8月前生产  
  \V3      V3 version (after 2018-08-01)2018年8月后
* * *
# How to update:
 (WIN7,WIN10,MAC,LINUX)
 * connect it to the PC
 * double click the RES button 
 * a new disk will display in you file explorer
 * copy the UF2 file in to the new disk.
 * the dongle will auto reset. Done.

# RCM-X86注入工具升级教程:
(支持WIN7,WIN10,MAC,Linux)
* 通过microUSB线(旧版本),或者USB口接到电脑
* 接到电脑后,双击RES 复位按钮.
* 此时会在我的电脑显示一个名为RCM 的U盘,
* 把相应的文件升级文件(大气层HBL或者OS,)拷贝进去即可，
  拷贝进去后会自动重启，拔出就可以使用了

* * *

If you don't know how to hack you switch,see this   
[How to use](https://github.com/euclala/RCM_typeC_ex/tree/master/jpg)

* * *

## 日志汇总 (BUG report)
* 注意,有部分版本硬件底层bootloader烧录有误,导致无法进入U盘模式.  
  如有此现象请与供应商联系.或者使用我提供的项目文件,用arduino编程软件进行烧录
* If you can not enter the update mode. maybe something wrong with the bootloader or the hardware.  
  See there to update.->>>  [FIX the dongle](https://github.com/euclala/fix_dongle)
  If you want to build you own payload , It's also by this way.
   

* * *

# Switch dongle RCM-X86 
RCM-X86 is MOD of Arduino Zero, 
It will send the Payload file to  NINTENDO SWITCH to run the Custom Firmware.(like Atmosphere,TX OS or others)
It was easy to change the dongle Firmware by PC,MAC or OS, using the UF2 files.

we have two version hardware:
* external dongle (with a battery, chagre 30minutes can payload about 500 times in 30 days.)
* internal dongle (solder it into the switch with 5-6 wire install,auto payload when the switch power on)
![res](https://github.com/euclala/RCM_typeC_ex/blob/master/jpg/reset_button.jpg)  

thanks for everyone in particular:
Atmosphere TEAM;@CTCaer;@mattytrog;@tumGER;@rajkosto;@Reisyukaku 
* * *



