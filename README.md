rpi-x-tools
===========

Compiled toolchain for raspberry pi, using crosstools-ng 1.19.0

Build was made with the following configurations of crosstools-ng-1.19.0. Build roadmap based on <a href = http://elinux.org/RPi_Linaro_GCC_Compilation</a> this manual

<h4>Paths & Misc:	</h4>
* Check <b>Try features marked as EXPERIMENTAL</b>	
* Set "Prefix directory" to whereever you want the finished toolchain to be placed	<b>(e.g. /home/romanjoe/x-tools)</b>
* Set "Number of parallel jobs" to be the number of processor cores in your system x1.5 -	<b>6</b>

<h4>Target options:</h4>	
* Set "Target architecture"	<b>ARM</b>
* Set Endianness" to <b>Little endian</b>
* Set "Bitness" to <b>32-bit</b>
* Set "Architecture level" to <b>armv6zk</b>
* Set "Emit assembly for CPU" to <b>arm1176jzf-s</b>
* Set "Tune for CPU" to	<b>arm1176jzf-s</b>
* Set "Use specific FPU" to	<b>vfp<b>
* Set "Floating point" to	<b>hardware (FPU)</b>
* Set "Default instruction set mode" to <b>arm</b>
* Check	Use EABI

<h4>General toolchain:</h4>	
* Set "Tuple's vendor string" to <b>rpi</b> - compiler vendor prefix
 
<h4>Operating system:</h4>	
* Set "Target OS" to <b>linux</b>
* Set "Linux kernel version" to <b>3.10.2</b>

<h4>Binary utilities:</h4>	
* Set "Binary format" to <b>ELF</b>
* Set "binutils version" to <b>2.23.1 (EXPERIMENTAL)</b>

<h4>C compiler:</h4>	
* Check "Show linaro versions"	
* Set "gcc version" to <b>linaro-4.8-2013.06-1</b>
* Check	<b>C++</b>
* Set "gcc extra config" to	<b>--with-float=hard</b>
* Check <b>Link libstdc++ statically into gcc binary</b>

<h4>C-library:</h4>	
* Set "C library" to <b>eglibc</b>
* Set "eglibc version" to <b>2_17</b>
