### Assignment #1

## Step 1: Environment Setup

### 1.1 VM Creation by Anandu
- **Action**: Created a VMware instance.
- **Details**: Enabled nested virtualization features.

### 1.2 Replication on Jeswanth's Laptop
- **Action**: Followed the initial setup steps.
- **Details**: Ensured the environment on Jeswanth's laptop mirrored Anandu's setup.

### 1.3 Forking the Kernel
- **Action**: Jeswanth forked the Linux kernel.
- **Details**: Obtained the latest Linux kernel source code from the repository for modifications.

## Step 2: Building the Kernel

### 2.1 Kernel Compilation
- **Action**: Compiled the updated Linux kernel.
- **Commands**:
  - `make oldconfig` for configuring the kernel with default old settings.
  - `make -j 8 modules` for building the kernel modules with parallel processing.

### 2.2 Final Build
- **Action**: Executed the final build process.
- **Command**: `make` to compile the entire kernel.

## Step 3: Code Modification

### 3.1 Base Code Setup
- **Action**: Imported base code from Canvas app.
- **Files Involved**:
  - `CMPE-283-1.c`
  - `makefile`

### 3.2 Feature Enhancements by Anandu
- **Action**: Extended `CMPE-283-1.c` with additional commands.
- **Commands Added**:
  - `IA32_VMX_PROCBASED_CTLS`
  - `IA32_VMX_PROCBASED_CTLS2`
  - `IA32_VMX_EXIT_CTLS`
  - `IA32_VMX_ENTRY_CTLS`
  - `IA32_VMX_PROCBASED_CTLS3`

## Step 4: Execution and Testing

### 4.1 Compiling the Program
- **Action**: Compiled the modified program in the home directory.
- **Command**: `make`

### 4.2 Module Insertion
- **Action**: Inserted the compiled module into the kernel.
- **Command**: `sudo insmod cmpe283-1.ko`

### 4.3 Verifying Output
- **Action**: Checked the kernel message buffer for output.
- **Command**: `sudo dmesg`

## Output Visuals

The results of the executed steps are illustrated in the screenshots below:

![Assignment Output 1](https://github.com/AnanduSreekumar/CMPE-283-Virtulization-Technologies/blob/main/Assignment-1/Screenshots/assignment_1.jpeg)

![Assignment Output 2](https://github.com/AnanduSreekumar/CMPE-283-Virtulization-Technologies/blob/main/Assignment-1/Screenshots/assignment_1_2.jpeg)
