## How to build
<br/>
I couldn't have done this if https://github.com/MichielDerhaeg/build-linux didn't exist.
<br/>
You will need some things before starting:
<br/>
* qemu
<br/>
* build-essential
<br/>
* musl-tools
<br/>
* grub-pc-bin
<br/>
<br/>
Installing build-esssentials, musl-tools, and grub-pc-bin:
<br/>
```sudo apt install build-essential musl-tools grub-pc-bin```
<br/>
<br/>
You will need to install qemu from: https://www.qemu.org/download/
<br/>
<br/>
Building AirLinux is very simple. Simply run:
<br/>
```make -j4 image```
<br/>
<br/>
Then, use qemu to run AirLinux virtually:
<br/>
```qemu-system-x86_64 -hds image```
