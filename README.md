# sdat2img
Convert sparse Android data image (.dat) to filesystem ext4 image (.img)



## Requirements
This binary requires Python 3.x installed on your system.

It currently supports Windows x86/x64, Linux x86/x64 & arm/arm64 architectures.



## Usage
```
sdat2img.py <transfer_list> <system_new_file> <system_ext4>
```
- `transfer_list` = input, system.transfer.list from rom zip
- `system_new_file` = input, system.new.dat from rom zip
- `system_ext4` = output ext4 raw image file



## Example
This is a simple example on a Linux system: 
```
~$ ./sdat2img.py system.transfer.list system.new.dat system.img
~$ mkdir output
~$ sudo mount -t ext4 -o loop system.img output/
```




## Info
For more information about this binary, visit http://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952.
