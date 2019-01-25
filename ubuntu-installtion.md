# Ubuntu Installation
1. Download Ubuntu 17.10 .iso file (bottom of the page) here: https://www.ubuntu.com/download/desktop
1. Installing Ubuntu 17.10 on Virtual Machine:
  *	Create your first virtual machine, refer: https://www.virtualbox.org/manual/ch01.html#gui-createvm
  * Minimum recommended disk space of virtual memory: 15 GB

Note: Although it is not necessary to create a virtual machine that matches the minimum specs required for ubuntu installation, you may refer to them here: https://help.ubuntu.com/community/Installation/SystemRequirements

Since Oracle VM VirtualBox allocates the portion of the host machine's RAM to the virtual machine, it is important to strike a balance between the minimum required specs for Ubuntu vs allocable RAM for the virtual machine.

  * Run your virtual machine by double-clicking on the entry within the manager window (or by selecting it and clicking on 'start')
  * If you are running your virtual machine for the first time you will be asked to select the path to the downloaded Ubuntu 17.10 .iso file (to install the OS in the virtual machine)
  * Follow the instructions and install Ubuntu with the default settings
  *	Alternatively you could select 'Something else' in the 'Installation type' screen to customize your installation with different memory allocation (for better performance), refer: https://askubuntu.com/questions/343268/how-to-use-manual-partitioning-during-installation

Note: Create swap area twice as big as the RAM size of virtual machine. Example: if virtual memory RAM is 2 GB then swap area should be 4GB

3. Installing Ubuntu in dual boot mode:
  * Create a bootable USB stick:
    1. Using windows: https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-windows#0
    1. Using Mac OS: https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-macos#0
  * Backup all data on your system
  * Dual boot with windows: https://help.ubuntu.com/community/WindowsDualBoot
    1. Additional documentation: https://www.lifewire.com/ultimate-windows-8-1-ubuntu-dual-boot-guide-2200654
  * Dual boot with Mac OS: https://www.lifewire.com/dual-boot-linux-and-mac-os-4125733
