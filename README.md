# A Kernel Seedling

A kernel module that counts the number of running processes and adds it to a file in /proc.

## Building

Run ```make``` to build the kernel module and ```sudo insmod proc_count.ko``` to load the module into the kernel.

## Running

Run the code with the command ```cat /proc/count``` It will print to the terminal an integer that represents the number of processes that are currently running. We can also look at the information messages printed in the kernel with ```sudo dmesg -l info```

## Cleaning Up

Remove the kernel module by running ```sudo rmmod proc_count``` Clean the code with ```make clean```

## Testing

Run the provided test cases with ```python -m unittest``` I tested my module on kernel release 5.14.8-arch1-1.

