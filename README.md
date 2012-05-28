linux-2.6-n2200
===============

Linux 2.6 on netvista (N2200)

Install linux on a Netvista (model n2200 8363 [1])

* Based on debian 5.0 (currently oldstable)
* Using gcc 3.4 as compiler

Building the kernel:

1. Apply video patch: linux-2.6-n2200-video.patch
2. Use linux-2.6.20-n2200.config as .config
3. Build bzImage and modules
4. Set byte 0x2c to 0x01 in arch/i386/boot/compressed/vmlinux
5. Copy kernel (arch/i386/boot/compressed/vmlinux) to netvista (/kernel.2x00)
   and modules

[1] https://www.google.com/search?tbm=isch&hl=en&q=netvista+n2200)
