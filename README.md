PreReqs
-
* [Keil uVision5 or armcc](http://www2.keil.com/mdk5/install/) - yes you need a licensed copy
* [cmake](https://github.com/ARMmbed/ble/issues/177)
* [srecord](https://sourceforge.net/projects/srecord/files/srecord-win32/) and put in your path
with `setx PATH "%PATH%;C:\Program Files\srecord"`
* [make](http://gnuwin32.sourceforge.net/packages/make.htm) -- download 'setup program' to get the dlls and put in your path with `setx PATH "%PATH%;C:\Program Files\GnuWin32\bin"`

Dependencies
-
Last upstream commit was Oct 2 2015 so I looked up commits from before then on the following source dependencies
* https://github.com/mbedmicro/mbed/releases?after=mbed_lib_rev108
* https://github.com/ARMmbed/ble/releases?after=v1.0.0 - NOTE I renamed BLE.h https://github.com/ARMmbed/ble/issues/177
* https://github.com/ARMmbed/ble-nrf51822/releases?after=v1.1.0

Build
-
* git clone git@github.com:jacobrosenthal/nrf5x-dfu-bootloader.git
* cd nrf5x-dfu-bootloader
* mkdir build
* echo $null >> .feedback
* cmake .. -G "CodeBlocks - Unix Makefiles"
* make VERBOSE=1

