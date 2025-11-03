--------------- LINUX QEMU NOTES ------------

These qemus are running a linux kernel, setup with options to work the the qemu machine type chosen for the qemu emulation(in the mips case, the 'malta' machine type)


There are a few scripts within the archive:

1) RUN_ME.sh - run the qemu, no wait for an external debugger

2) RUN_DBG.sh - run the qemu, waiting for an external gdb to connect to 'localhost:1234'  (use this if you want to debug at the kernel level)

3) mount.sh - use this to 'mount' the rootfs (filesystem) to the 'out' folder, you can add/modify/copy off etc any files from this rootfs


files in the archive:  

image_xxxx.raw:  rootfs filesystem 

vmlinux_xxxxx:  linux kernel image (w/debug symbols, can load this into gdb)

run_me.sh/run_dbg.sh/mount.sh:  scripts for running, etc

