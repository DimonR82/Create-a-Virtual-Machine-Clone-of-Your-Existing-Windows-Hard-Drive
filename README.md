#Create a Virtual Machine Clone of Your Existing Windows Hard Drive

Virtualization allows one operating system (OS) to run on another OS. But did you know that a Virtual Machine (VM) clone of your hard drive can put your entire computer inside of another computer? With VMs, the possibilities are endless. For most people, though, virtualization enables playing older games using emulation, the ability to sandbox, running multiple operating systems, and much more.


Thanks to virtualization and virtual machines, you can run any operating system on your PC. On a Windows PC, this could mean being able to run a Linux distribution or even macOS without messing with your main computer. Read on as we detail how you can create a VM clone of your system and how to use it once you've managed to create the virtual machine.

How to Create a Virtual Machine Clone
-------------------------------------

Creating a VM clone is simple thanks to Microsoft's [Disk2VHD](https://technet.microsoft.com/en-us/sysinternals/ee656415.aspx) or [CloneVDI](https://forums.virtualbox.org/viewtopic.php?t=22422). Disk2VHD creates a copy of your installed software that runs on software known as a [virtual machine](https://www.makeuseof.com/tag/virtual-machine-makeuseof-explains/). A virtual machine fakes the environment of a physical computer.


Think of it as a holodeck for software. Once created, the duplicated image can work on any hardware with a VM installed. While Disk2VHD creates a copy of your hard drive's contents, it doesn't function as a system backup.

How to Create a Virtual Machine From a Windows 10 Disk
------------------------------------------------------

Disk2VHD requires very little space, works on Windows Vista and later, and doesn't require installation as it's a portable app. The below method details how you can create a VHD from a physical disk on Windows 10 using Disk2VHD:

googletag.cmd.push(function() { googletag.display('div-gpt-ad-1494450502098-ccr3'); });

1.  Download Disk2VHD from the [Microsoft Docs website](https://docs.microsoft.com/en-us/sysinternals/downloads/disk2vhd) and extract the contents of the zipped file.
2.  Right-click on **Disk2vhd.exe** and click on **Run as administrator** from the context menu.
3.  When prompted to provide **User Account Control**, click on **Yes.**
    
        
    
4.  Be aware that the VHDX file format isn't supported by all Virtual Machine software. You may want to uncheck **Use Vhdx** if you aren't sure your software supports it.
5.  Finally, select the disk volume you want to clone and click on **Create**.

googletag.cmd.push(function() { googletag.display('div-gpt-ad-1494450502098-ccr4'); });

In the **Space Required** column, Disk2VHD shows you the amount of hard disk space you will need to have in order to create the virtual hard disk from your computer's partitions. The larger the partition, the longer the process takes.

Furthermore, the process creates a complete copy of your system, so you need at least double the space required. For example, if your C:\\ takes up 140 GB, you will need at least 140 GB of free space. The cloning process can take a long time, depending on your processor's speed and the size of your installation.

googletag.cmd.push(function() { googletag.display('div-gpt-ad-1494450502098-ccr5'); });

Once you have created the VHD file, you can use a virtualization app to run it. Several VM programs exist, but [VirtualBox](https://www.virtualbox.org) and [VMware's Workstation Player](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) are the most popular and reliable.

Related: [VirtualBox vs. VMWare vs. Hyper-V: What's the Best Virtual Machine?](https://www.makeuseof.com/tag/virtualbox-vs-vmware-vs-hyper-v/)

How to Run a Windows 10 Virtual Machine Image
---------------------------------------------

There are two ways that you can access the contents of a VHD file. Windows, from Vista on, can directly explore within a VHD file by double-clicking on it (most of the time, see below).

The second method, booting a VHD file from within a VM, requires a bit more effort -- and it isn't worth the effort to make the image bootable.

To get started browsing the files of a VHD:

1.  Launch the **Start** menu, search for **Disk Management**, and then click on the Best match. In the Windows 10 Start menu search bar, **Disk Management** is labeled as **Create and format hard disk partitions** instead.
2.  Within **Disk Management**, click on **Action** from the toolbar menu and then select **Attach VHD.**
    
        
    
3.  Click on **Browse** and then navigate to the directory where you stored the VHD file.
4.  Select it and then click **OK**.

googletag.cmd.push(function() { googletag.display('div-gpt-ad-1494450502098-ccr-REPEAT6'); });

Unless you changed its default location, the VHD file gets created inside of the Disk2VHD folder. That's more than likely inside of your **Downloads** directory.

Once you've selected the VHD file, the image will attach itself to your Windows system and become available as a standalone disk. You can then browse it as you would an external drive.

Cloning a Hard Drive to a Virtual Machine, Made Easy
----------------------------------------------------

You cannot boot from a VHD on a PC without acquiring another Windows license, but an image of your OS retains essential files that you can always restore in the event of a catastrophic data loss. Once you have cloned a hard drive, you can always run it using virtual machine software.
