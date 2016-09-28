#how to install
#############################
cd rtl8723bu

sudo make

sudo make install

sudo reboot
#############################

lsmod |grep 8723bu

##############################

#if it doesn't work ,you need to check wheather the interface is using another driver

dmesg |grep [wlan interface name]

#the promt should like this

[    3.705130] < drive name > 1-6:1.2 <interface name>: renamed from wlan0

#if not  , disable the wrong driver
