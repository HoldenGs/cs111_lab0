# A Kernel Seedling

Kernel Seedling is a kernel module that creates a virtual file at /proc/count.
The contents of this file contains a string that displays the
number of currently running processes.

## Building

Explain how to build your kernel module

To build the kernel module, you can simply run

```
make
```

## Running

Explain how to run your kernel module and what to expect

This module is designed to run on Arch Linux. It may not work
as expected on other platforms. To insert the module, simply
run:

```
sudo insmod proc_count.ko
```

After running `make`.

## Cleaning Up

Explain how to remove your kernel module and clean up the code

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

