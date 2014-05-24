# You should only have to change this value:
PORT = /dev/tty.usbserial-DNWYFIDM

# You should only set the path to your Arduino application if it is not in your path or not the default one:
# The default for Linux and Solaris is:
#ARD_HOME = /opt/Arduino
# The default for Mac is:
#ARD_HOME = /Applications/Arduino.app

# Uncomment to activate serial debugging for the USB Host library:
#EXTRA_FLAGS += -D DEBUG_USB_HOST

# Leave these alone
all: 
	arm-linux-gnueabihf-g++ -D__ARM_ARCH_7A__ -I/home/ubuntu/usr/xenomai/include -D_GNU_SOURCE -D_REENTRANT Balanduino.h  Kalman.h EEPROMAnything.h  I2C.c   Tools.c Balanduino.c Bluetooth.c  EEPROM.c Kalman.h  Motor.c Spektrum.c -D__XENO__  -Xlinker -rpath -Xlinker /home/ubuntu/usr/xenomai/lib -lnative -L/home/ubuntu/usr/xenomai/lib -lxenomai -lpthread -lrt -v -o bal
