# 2.11BSD-ingres
2.11BSD image with ingres kernel support compiled in and ingres compiled

# Credits:

Starting point is Chase Covello and Jeff Thiekle's 2.11BSD image disk that contains patch level 482, the kernel source code and the ingres source code:

https://github.com/chasecovello/211bsd-pidp11

They did all the work to give us a full featured 2.11BSD image with everything working out of the box

The code fix for compiling the ingres database successfully is from Heinz-Bernd Eggenstein:

https://groups.google.com/g/pidp-11/c/xQByLmGWARo

Included fixes:

- created an INGRES config for the kernel to include INGRES YES
- kernel Makefile overlay modification so that kernel compiles without errors
- modifications to the ingres ovqp source code to change const into const_ so that ingres compiles
- password for the ingres user set to Ingres
- added tape device (TQ0) to the boot.ini for easy transfer of files go here to find how to use and convert .tar to a format usable by BSD: https://github.com/rricharz/pidp11-2.11bsd

# Download

The disk image is in the release section, here is a direct link to the image: https://github.com/slajeune/2.11BSD-ingres/releases/download/v1.0.0/2.11BSD_rq.dsk.xz

# Ingres on pip-11

This is a good starting point for ingres on pip-11

https://pdp2011.sytse.net/wordpress/ingres/
