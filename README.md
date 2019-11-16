# Supercon_2019
## Stuff from Supercon 2019

### Reflash badge:

dfu-util -a 0 -D soc.bit
dfu-util -a 1 -D ipl.bin


### load the blinky program in place of the initial menu program
### it's the same line as in the Makefile but change the "-a 2" to "-a 0"

dfu-util -d 1d50:614a,1d50:614b -a 0 -R -D blinky.bit


