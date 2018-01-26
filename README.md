# rtl8821ce
wireless driver  
https://github.com/endlessm/linux/tree/master/drivers/net/wireless/rtl8821ce  
Thinkpad E470c, Realtek 8821CE Wireless LAN 802.11ac PCI-E NIC  

Unpack zip archive.  
Change the Makefile. Line "export TopDIR ?= ..." to export "TopDIR ?= PATH TO EXTRACTED DIRECTORY".  
make  
sudo make install  
sudo modprobe -a 8821ce  


要求内核高于4.11,ubuntu16内核最高好像是4.10，需要自己升级内核版本  
两个链接是linux内核链接和下载链接  
Makefile文件中把 "export TopDIR ?= ..." to export "TopDIR ?= PATH TO EXTRACTED DIRECTORY" 就是填写当前路径地址  
最后一步可能说没有钥匙什么的，需要关闭BIOS中的Secure Boot。关闭之后就OK   
