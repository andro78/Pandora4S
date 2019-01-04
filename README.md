# Pandora4S
Pandora4S kernel

Pandora 4S has 2 partitions - can see in linux system only. (I checked Raspberry Pi)
1. Use USB reader for reading SD card.
2. Dump SD card in PB4 by 'USB Image Tool'.(size : 7.40GB)


--------------------------------------------------------------
1. Start: 

myinit

#!/bin/sh

export PATH=/bin:/sbin:/usr/bin:/usr/sbin:/usr/local/bin:/usr/
export LD_LIBRARY_PATH=/lib:/usr/lib:/usr/local/lib

export QWS_DISPLAY=LinuxFb:/dev/fb0
export QTDIR=/root/real210/qt3

sleep 1

while true
do
	/usr/emu/emulotar
done
