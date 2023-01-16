# A Kernel Seedling

Kernel Seedling is a kernel module that creates a virtual file at /proc/count.
The contents of this file contains a string that displays the
number of currently running processes.

## Building

To build the kernel module, you can simply run

```
make
```

## Running

This module is designed to run on Arch Linux. It may not work
as expected on other platforms. To insert the module, simply
run:

```
sudo insmod proc_count.ko
```

After running `make`.

## Cleaning Up

To remove the module and delete the virtual file, run:

```
sudo rmmod proc_count.ko
```

## Testing

This code is tested on release 5.14.8-arch1-1 of Arch Linux.
It is not guaranteed to work on any prior or later versions.
To test the module, you can run:

```
python -m unittest
```

The expected output is 3 successful tests.

Be aware that tampering with module code can cause the system to enter
into failure modes from which the only recourse is to delete and reinstall
your machine. As such, you are encouraged to thoroughly test this code
in a VM before using it in your daily machine.

