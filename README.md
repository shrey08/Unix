# Unix
Using CentOS 7 on VirtualBox 

Post Installation:

-To update the softwares:
   Method 1. Go to Applications -> Sofware Tools -> Application Installer OR Applications -> Sofware Tools -> Software Updates.
   Method 2. Go to Applications -> Terminal
             Type command: sudo yum update (This will update your packages)

-Take the snapshot of updated system using, (right ctrl+t)

-Now, to install Development Tools:
   Type command: sudo yum groupinstall "Development Tools"
   
-To install VirtualBox Guest Addition:
   From "Devices" option choose "Insert Guest addition CD image". Then Run it and after completion, reboot the system.
   In the "View" check if Auto-resize Guest Display is enabled or not.
   
   If it is not enabled and couldn't be accessed then open the Terminal.
             Type command: sudo yum install gcc make kernel-devel bzip2 binutils patch libgomp glibc-headers glibc-devel kernel-headers -y
   After executing this command repeat the above steps of installing VirtualBox Guest Addition.

-Customize GNOME 3 Desktop:
   First we need to install the plugin.
            Type command: sudo yum install gnome-shell-browser-plugin
   After executing this command, open your browser and go to "https://extensions.gnome.org" and install any extension you want. 
