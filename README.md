# A Kernel Seedling

This is a module that creates a virtual file at /proc/count.
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

To remove the module and delete the file, run:

```
sudo rmmod proc_count.ko
```

## Testing

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

