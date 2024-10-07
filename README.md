# kali-install-macos
Installation Instructions for Kali Linux on a VM on MacOS

# 1. Download Required Files
You will need to download 3 different files.
1. [VirtualBox](https://download.virtualbox.org/virtualbox/7.1.2/VirtualBox-7.1.2-164945-macOSArm64.dmg)
2. [VirtualBox Extension Pack](https://download.virtualbox.org/virtualbox/7.1.2/Oracle_VirtualBox_Extension_Pack-7.1.2.vbox-extpack)
3. [Kali Linux .iso Installer File](https://cdimage.kali.org/kali-2024.3/kali-linux-2024.3-installer-arm64.iso)

# 2. Install VirtualBox
Run the `VirtualBox-x-macOSArm64.dmg` installer file you downloaded in the previous step.
Follow all on-screen propts for a standard installation.

# 3. Create the Kali Linux VM
Click on the blue star button at the top of the window labelled 'New'. Enter a name for the installation, I use `Kali Linux` so I know what I'm installing but feel free to go with something else. For the ISO Image, click on the blue dropdown arrow, click on the `Other` option, and navigate to where you downloaded the `.iso` installer image file earlier.

If the installer image file has been imported successfully, the `Type`, `SubType`, and `Version` fields should be populated with `Linux`, `Ubuntu`, and `Ubuntu (ARM 64-bit` automatically and become disabled for editing.

For the Base Memory, a good minimum is 2048 MB (2 GB), however if your device has 16 GB of total ram, increase this number to 4096 MB (4 GB). Leave the number of processors at 1 CPU (all the way to the left), and check the box to enable EFI.

For the Virtual Hard Disk, a good minimum is 10 GB, however if your device has a higher total storage, feel free to increase this number.

Read through the summary at the end to make sure everything is configured correctly, then click finish to create the VM.

# Installing Kali Linux on the VM
Click on the new VM you just made on the left menu, it should be highlighted blue. Click on the settings cog at the top and scroll down to the display section. Change the scale factor to 200% so the VM window appears larger (it is very small by default). Click ok to apply this change, then click on the green start button at the top of the screen.

Click into the VM window and use the down arrow key to select the graphical install option and hit enter to select it.

Select your preferred language, then click continue. Choose your location, this will also be used to configure the local time later. Then select which keyboard layout you wish to use. Most keyboards in Australia use the American English keyboard layout so select it if it is the same for you.

Choose a hostname for the Virtual Machine, name it anything you wish to use and click continue. Do the same for your domain name. Enter your name and a username to set up the user account, then choose a password.

Choose the timezone where you are located, this would be determined by the country you selected earlier. Select the appropriate one then continue.

When prompted to partion the disk select the option `Guided - use entire disk` then click continue. It should show you the VBOX HARDDISK with the capacity you chose when setting up the VM, click continue to move on to partition the drive. Select the option to have all the files in one partion (which is recommended), thenc click continue. It will then give yoy an overview of the partitions being created, select the option to finish partitioning and write it to the disk. It will ask you for a confirmation, select `yes` on the radio button and continue.

For the software selection, select `Desktop environment` and make sure it is the only option selected, then continue.

Once the installation completes, click continue to boot into the system. Once it loads, select the top option, then log in with the username and password you set during the installation.

# Congratulations!
If you have followed all of the steps, you would have been able to boot into a Kali Linux VM running on MacOS!
