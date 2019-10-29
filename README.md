# qemu-kzm-dtb
Device Tree for QEMU KZM Machine
## Background
I was looking to emulate a machine with an arm1136 CPU with QEMU. The only machine QEMU offers which natively supports the arm1136 CPU is the KZM machine. Unfortunately, the DTS file (imx31-lite.dts) that comes with the Linux kernel (tested with Linux 4.19.80) does not support networking on the KZM machine included in QEMU. The DTS/DTB file provided in this repo enables networking on this machine. Unfortunately QEMU has not yet implemented disk drivers (PATA) on this machine, however with the ability to utilize networking now, you can netboot this machine.
