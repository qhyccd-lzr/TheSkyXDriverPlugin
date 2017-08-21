# TheSkyXDriverPlugin
This is so called Software Bisque's X2 driver needed for TheSkyX. Runs on Ubuntu Linux with Intel processors as well as on Raspberry PI3 and Odroid XU4 embedded machines.

How to use it:
1) There are two targz files. The first one named qhyccdx2plugin-1.x.x-linux.tar.gz is used on Intel processors and Ubuntu Linux, while the second one named qhyccdx2plugin-1.x.x-rpi3-gcc-4.9.tar.gz is used on ARM V8 processors (RPI3, Odroid XU4).
2) Copy an appropriate file to the place where your TheSkyX is installed.
3) Untar the targz file using: tar xzvf file_name.tar.gz
4) Go to its install_scripts directory and run an appropriate installation script. The first one contains word "shared", the second one word "static" inside its script names. The "shared" script will install the X2 driver which will be link with libqhy.so library on run time, while the "static" script will install the X2 driver which is already statically linked with libqhy.a library. User can select whatever version he/she wants, but if "shared" solution is selected, it is necessary to install the libqhy.so driver too.
