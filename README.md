# 9100F_B360i_GT730_OC

------------------基本配置---------------------------------------  
主板｜ROG STRIX B360-I GAMING  
CPU｜Intel(R) Core(TM) i3-9100F  
内存｜Galaxy 8G 2133MHZ x 2  
硬盘｜SAMSUNG SM963 NVMe 480GB  
显示｜Dell U2419Q（DisplayPort）  
显卡｜Bitland NVIDIA GeForce GT 730 2G（HP拆机）  
声卡｜Realtek 1220A SuperFX  
有线｜Intel i219v7 Gigabit Ethernet  
无线｜BCM943224PCIEBT2（替换自带的英特尔9560AC)  

------------------工作设备---------------------------------------  
声卡：		                     OK  
显卡：		                     OK  
有线：		                     OK  
无线：		                     OK  
睡眠：		                     OK  
唤醒：		                     OK  
AirDrop ：	                  OK  
Handoff ：	                  OK  
FaceTime：                 	OK  
iMessage ：	                OK  

------------------BIOS设置---------------------------------------  
BIOS版本：	2811 （2020/07/23）  
CFGLock>>Disabled  
VT-d>>Disabled  
大于4G地址空间解码>>Enabled  
DVMTPre-Allocated>>128M（如果有）  
Systemtime and Alarm Source >>Legacy RTC  
SATA模式选择>>AHCI（必须设置）  
legacyUSB support>>Enabled  
XHCIHand-off>>Enabled  
快速启动>>Disabled  
开启CSM>>Disabled  
安全启动状态>>关闭  
操作系统类型 >>其他操作系统  

------------------OpenCOre---------------------------------------  
2021.1.11  
1、更新版本到0.6.5  
2、定制USBX和USBPorts，其中11和14接口为AURA控制器和蓝牙控制器，  
前置5和6接口没有使用  
3、KEXT包含AirportBrcmFixup.kext以支持943224在OSX10.15和  
OSX11.0中驱动无线  
4、Kernel>Patch>0分支下添加了华硕主板重启卡F1的补丁  
5、PlatformInfo>Generic>分支下的三码已经清除，自行添加iMacPro1,1  
