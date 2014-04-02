rpi-x-tools
===========

Compiled toolchain for raspberry pi, using crosstools-ng 1.19.0

Build was made with the following configurations of crosstools-ng-1.19.0:

<h2>Paths & Misc:	</h2>
Check "Try features marked as EXPERIMENTAL"	
Set "Prefix directory" to whereever you want the finished toolchain to be placed	(e.g. /home/romanjoe/x-tools)
Set "Number of parallel jobs" to be the number of processor cores in your system x1.5	6
Target options:	
Set Target architecture	ARM
Set "Endianness" to	Little endian
Set "Bitness" to	32-bit
Set "Architecture level" to 	armv6zk
Set "Emit assembly for CPU" to	arm1176jzf-s
Set "Tune for CPU" to	arm1176jzf-s
Set "Use specific FPU" to	vfp
Set "Floating point" to	hardware (FPU)
Set "Default instruction set mode" to 	arm
Check	Use EABI
General toolchain:	
Set "Tuple's vendor string" to	"rpi"compiler vendor prefix
Operating system:	
Set "Target OS" to	linux
Set "Linux kernel version" to 	3.10.2
Binary utilities:	
Set "Binary format" to 	ELF
Set "binutils version" to 	2.23.1 (EXPERIMENTAL)
C compiler:	
Check "Show linaro versions"	
Set "gcc version" to 	linaro-4.8-2013.06-1
Check	C++
Set "gcc extra config" to	--with-float=hard
Check 	Link libstdc++ statically into gcc binary
C-library:	
Set "C library" to	eglibc
Set "eglibc version" to 	2_17
Далее:	
Зарегистрировать путь к новому компилятору	PATH=$PATH:/home/romanjoe/x-tools/bin
Проверить, зарегистирован ли новый компилятор	arm-rpi-linux-gnueabi-gcc -v
