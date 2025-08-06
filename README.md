# 2.11BSD-ingres
2.11BSD image with ingres kernel support compiled in and ingres compiled

# Credits:

Starting point is Chase Covello and Jeff Thiekle's 2.11BSD image disk that contains patch level 482, the kernel source code and the ingres source code:

https://github.com/chasecovello/211bsd-pidp11

They did all the work to give us a full featured 2.11BSD image with everything working out of the box

The code fix for compiling the ingres database successfully is from Heinz-Bernd Eggenstein:

https://groups.google.com/g/pidp-11/c/xQByLmGWARo

Included fixes:

- create an INGRES config for the kernel to include INGRES YES
- kernel Makefile overlay modification so that kernel compiles without errors
- changes to the ingres ovqp to change const into const_ so that ingres compiles
- password for the ingres user set to Ingres
- added tape device (TQ0) to the boot.ini for easy transfer of files go here to find how to use and convert .tar to a format usable by BSD: https://github.com/rricharz/pidp11-2.11bsd
