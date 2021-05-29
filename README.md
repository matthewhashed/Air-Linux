## How to build
I couldn't have done this if https://github.com/MichielDerhaeg/build-linux didn't exist.  
You will need some things before starting:  
* qemu
* build-essential
* musl-tools
* grub-pc-bin  
Installing build-esssentials, musl-tools, and grub-pc-bin:  
```sudo apt install build-essential musl-tools grub-pc-bin```  
  
You will need to install qemu from: https://www.qemu.org/download/  
  
Building AirLinux is very simple. Simply run:  
```make -j4 image```  
  
Then, use qemu to run AirLinux virtually:  
```qemu-system-x86_64 -hds image```
