

## Questions

### Assignment 2 (0x4FFFFFFF) & (0x4FFFFFFC)

1. **Team Contribution**
   
Anandu - Prepared the nested VM environment and coded the leaf node 0x4FFFFFFC. 
Jeswanth - Coded the leaf node 0x4FFFFFFF, created the testing program, and checked the validity of the results.
    
2. **Describe in detail the steps you used to complete the assignment.**
   

## Getting the Linux Kernel Source
I can help you with paraphrasing your text in a high-quality English. Here is one possible way to rewrite your text:

## Obtaining the Linux Kernel Source

1. **Clone the Linux Kernel Repository:**
    ```bash
    git clone https://github.com/jeswanthv/linux.git
    ```

2. **Go to the Linux Directory:**
    ```bash
    cd linux
    ```

3. **Install the Necessary Packages:**
    ```bash
    apt-get install virt-manager build-essential kernel-package fakeroot libncurses5-dev libssl-dev ccache bison flex libelf-dev
    ```

4. **Copy the Boot Config File to the Linux Folder:**
    Replace `("Your_VM_Version")` with your actual VM version.
    ```bash
    cp /boot/config-("Your_VM_Version") .config
    ```

5. **Make Old Configuration:**
    ```bash
    make oldconfig
    ```

6. **Build Kernel Modules:**
    ```bash
    make -j 8 modules
    ```

7. **Build the Kernel Image:**
    ```bash
    make prepare
    make -j 8
    ```

8. **Install the Modules:**
    ```bash
    sudo make INSTALL_MOD_STRIP=1 modules_install && sudo make install
    ```

9. **Reboot the VM:**
    ```bash
    reboot
    ```

10. **Verify the Kernel Module Name Change:**
    ```bash
    uname -a
    ```

11. **Remove the KVM and KVM_INTEL Modules:**
    ```bash
    rmmod kvm_intel
    rmmod kvm
    ```
12. **Update the KVM and KVM_INTEL Modules:**
  ```bash
    modprobe kvm
    modprobe kvm_intel
    lsmod | grep kvm
    ```
13. **Run the command sudo virtmanager**
    ```sudo virt-manager
    ```
