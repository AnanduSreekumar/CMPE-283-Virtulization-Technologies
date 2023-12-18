Step 1 - Setup
a. Anandu Created a VM Ware with nexted virtulization enabled 
b. Followed the steps and recereted in Jeswanth Laptop
c. Jeswaznth focked the linux kernel code

Step 2 - Building the kernel 
a. Build the kernel with the updated version in the linux repo using make oldconfig and make -j 8 modules
b. Ran make command

Step 3 - Code Modification
a. Copied the base code from canvas app (CMPE-283-1.c and makefile)
b. Anandu edited CMPE-283-1.c with other 5 commands(IA32_VMX_PROCBASED_CTLS,IA32_VMX_PROCBASED_CTLS2,IA32_VMX_EXIT_CTLS,IA32_VMX_ENTRY_CTLS,IA32_VMX_PROCBASED_CTLS3)

Step 4 - Run File
a. Make command in home directory
b. sudo insmod cmpe283-1.lko
c. sudo dmesg

Output:

<img align="center" src="https://github.com/AnanduSreekumar/CMPE-283-Virtulization-Technologies/blob/main/Assignment-1/Screenshots/assignment_1.jpeg" alt="Homepage" height="305" width="620" />
 
<img align="center" src="https://github.com/AnanduSreekumar/CMPE-283-Virtulization-Technologies/blob/main/Assignment-1/Screenshots/assignment_1_2.jpeg" alt="Homepage" height="305" width="620" />

