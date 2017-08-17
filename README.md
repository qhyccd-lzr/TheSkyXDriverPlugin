# TheSkyXDriverPlugin
This is so called X2 driver reqired by Software Bisque's TheSkyX. Runs on Intel Linux as well as Raspberry PI3 and Odroid XU4 embedded machines.

How to use it:
1) There are two targz file, the first one named qhyccdx2plugin-1.0.0-linux.tar.gz is used on Ubuntu Linux, while the second one named qhyccdx2plugin-1.0.0-rpi3-gcc-4.9.tar.gz is used on ARM processors.
2) Copy an appropriate file to directory where your TheSkyX is installed.
3) Untar targz file there using tar xzvf file_name.tar.gz
4) Go to its install_scripts directory and run an appropriate installation script. OThe first one is used for Linux, the second one for ARM.
./linux_install_qhyccdx2plugin.sh or ./rpi3_install_qhyccdx2plugin.sh
5) Start your TheSkyX.
