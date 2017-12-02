# TheSkyXDriverPlugin
Here are several distributions of Software Bisque's X2 driver needed by TheSkyX. Runs on Mac OSX, Ubuntu Linux with Intel processors as well as on Raspberry PI3 and Odroid XU4 embedded machines.

LINUX - how to install X2 driver:
---------------------------------
1) There are two targz files. The first one named qhyccdx2plugin-1.x.x-linux.tar.gz is used on Intel processors and Ubuntu Linux, while the second one named qhyccdx2plugin-1.x.x-rpi3-gcc-4.9.tar.gz is used on ARM V8 processors (RPI3, Odroid XU4).
2) Copy an appropriate file to the place where your TheSkyX is installed.
3) Untar the targz file using: tar xzvf file_name.tar.gz
4) Go to its install_scripts directory and run an appropriate installation script. The first one contains word "shared", the second one word "static" inside its script names. The "shared" script will install the X2 driver which will be link with libqhy.so library on run time, while the "static" script will install the X2 driver which is already statically linked with libqhy.a library. User can select whatever version he/she wants, but if "shared" solution is selected, it is necessary to install the libqhy.so driver too.

Mac OSX - how to install X2 driver:
-----------------------------------
1) Copy qhyccdx2plugin-1.x.x-macos-i386.tar.gz to the Contents subdirectory of your TheSkyX. In my case, TheSkyX is installed at: /Applications/TheSkyX Professional Edition.app, so I have to go to the Contents subdir: cd Contents
2) Untar the targz file there using: tar xzvf qhyccdx2plugin-1.x.x-macos-i386.tar.gz
3) Go to the install_scripts: cd qhyccdx2plugin-1.x.x-macos-i386/install_scripts/
4) Run installer: sudo ./macos_install_qhyccd_x2_driver.sh
5) Start TheSkyX and you should be able to connect to your QHYCCD camera. 

NOTE: This Mac OSX installer will install all the necessary stuff needed to operate your QHYCCD cameras on Mac OSX.
It doesn't require libqhy.dylib library for example, because everything is included inside the X2 driver itself.
This driver will install 32 bit libusb library inside the /usr/local/lib directory, and all firmwares inside the /usr/local/lib/qhy/firmware directory.

Please note, this first release is still under development. Send me an email to astrosoft AT email DOT cz in the case
of any problem. Thank you, JS
