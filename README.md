## UID: 005717129

## Building
To build the kernel module, navigate to the folder containing proc_count.c and Makefile and execute the make command.

## Running
After building the kernel module, insert it into the kernel by running sudo insmod proc_count.ko. Check the module's details by running modinfo proc_count.ko. To display the number of running processes, use the command cat /proc/count.

## Cleaning Up
To remove the kernel module, use the command sudo rmmod proc_count. This will unload the module from the kernel. Execute make clean to remove object and executable files and clean up the code.

## Testing
I tested my module on kernel release version 5.14.8-arch1-1, which I confirmed by running the command uname -r. To view information about the kernel release version being tested, use the command modinfo proc_count.ko.
