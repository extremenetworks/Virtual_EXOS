# Setting up GNS3 with EXOS-VM in macOS
This Guide will assist you in setting up GNS3 V2 and above to work with EXOS-VM on macOS.  If you have any questions about this guide please open a [Issue](https://github.com/extremenetworks/Virtual_EXOS/issues/new) on GitHub or on  [The HUB](http://community.extremenetworks.com/).  

**Note: EXOS-VMs can get stuck in (pending AAA) for 1-2 minutes.  Just be patient it will finish, and allow you to login**.

### What you will need: -- See "Getting Started" section below for step by step instructions.
* Vmware Fusion - latest version  --  This is needed for the GNS3-VM
 	* https://www.vmware.com/products/fusion
	
* GNS3-VM.ova from GitHub  --  This version must match the version of GNS3 on your local machine
 	* GNS3.VM.VMware.Workstation.X.X.X.zip
 		*  https://github.com/GNS3/gns3-gui/releases

* GNS3 for your local machine.  -- This version must match the version of GNS3-VM
 	*  GNS3-X.X.X.dmg
 		*  https://www.gns3.com/software/download or https://github.com/GNS3/gns3-gui/releases

* GNS3 Template File for EXOS VM  -- This is used to import EXOS into GNS3
	* exosvm.gns3a
		* https://github.com/extremenetworks/Virtual_EXOS/blob/master/exosvm.gns3a?raw=true

------
### Getting Started:

#### Step 1: Download GNS3 Template File
* Download GNS3 Template File for EXOS VM.  --  You will need this in Step 7  
	* https://github.com/extremenetworks/Virtual_EXOS/blob/master/exosvm.gns3a?raw=true  *"right-click save link as"*

#### Step 2: VMware Fusion

* Download and install [VMware Fusion](https://www.vmware.com/products/fusion). 

#### Step 3: GNS3-VM.ova
1.  Download [GNS3.VM.VMware.Workstation.X.X.X.zip](https://github.com/GNS3/gns3-gui/releases) from GitHub  -- This version must match the version of GNS3 program on your local machine
2.  Import the GNS3-VM.ova into VMware Fusion.  **Don't start it yet.**
3.  Edit the VM to make sure you give it as much memory and CPUs as you can.  This will help improve your experience when using GNS3 and EXOS-VM.  I recommend giving the VM half of your CPUs and half of your RAM.
4. Boot up VM and note the IP it gets.  Keep the VM up.

#### Step 4: GNS3 for your local machine
* Download [GNS3-X.X.X.dmg](https://www.gns3.com/software/download), mount it, and copy GNS3.app to `/Applications/`  -- This version must match the version of GNS3-VM

#### Step 5: Open GNS3
1. Make sure GNS3-VM is booted
2. Open GNS3

#### Step 6: Setting up GNS3
1. When initially opening GNS3, it will prompt you to authenticate with an admin account to allow uBridge root permissions (for interacting with network interfaces). Allow root access for uBridge and authenticate as an admin user.
2. GNS3 will automatically detect and connect to the GNS3 VM.

#### Step 7: Import EXOS-VM as Appliance 
1. Go to File -> Import appliance -> Open the exosvm.gns3a file downloaded in Step 1.
2. Click next -> Select "Run the appliance on the GNS3-VM" -> Click next.
3. You should see multiple versions of EXOS.  Expand the version you want and click on the file. -> click Download.
4. Once downloaded, click Refresh, then select the version and click Next. When prompted, answer Yes to install.
5. Now you will see a switch that is called "EXOS VM XX.X.X.X" in your inventory.
6. Drag the VM to your project. and select yes to upload your image to your VM.
7. Repeat these steps as needed to install all the desired versions of EXOS VM.

### Step 8: Have fun!
1. Move more switches over connect them together, boot them up, and configure them.  Be careful for loops!

### Screenshot

<img src="GNS3_macOS.png">
