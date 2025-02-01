Pi Zero expansion board with ethernet, USB Type-C and 3.3 V regulation for high current additions. 
Features enough space for any additions. 
The PCB is 4 Layer with 2 inner layer being +5V and GND

Ethernet connection is done by using ENC28J60 
To enable it on Pi zero change /boot/firmware/config.txt
Uncomment 
dtparam=spi=on 
and below add 
dtoverlay=enc28j60

reboot and verify eth0 interface by running ifconfig command 
