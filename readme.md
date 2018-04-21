## about rtl8821ce
https://github.com/endlessm/linux/tree/master/drivers/net/wireless/rtl8821ce  
Thinkpad E470c,  
wireless driver  
Realtek 8821CE Wireless LAN 802.11ac PCI-E NIC  

## install  
1. Edit the Makefile / 编辑Makefile  
Line "export TopDIR ?= ..." to "export TopDIR ?= PATH TO EXTRACTED DIRECTORY".  

2. Kernel version / 内核版本,源项目更新最新的源代码或许能支持更新的内核  
sudo uname -r  
4.11-->  
4.13.0-37-generic  

3. BIOS Trun off the Secure Boot /BIOS关闭Secure Boot  

4. make & Install /编译安装  
make  
sudo make install  
sudo modprobe -a 8821ce  
