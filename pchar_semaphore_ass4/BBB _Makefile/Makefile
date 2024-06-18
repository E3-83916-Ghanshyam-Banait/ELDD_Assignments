
obj-m = gpio-led-switch.o

modules:
	make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- -C /home/ghanshyam/linux/ M=`pwd` modules
	
copy:
	scp gpio-led-switch.ko debian@192.168.7.2:/home/debian
clean:
	make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- -C /home/ghanshyam/linux/ M=`pwd` clean		
	
.PHONY: all clean

