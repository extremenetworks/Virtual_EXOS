# Setting up GNS3 with EXOS-VM
This Guide will assist you in setting up GNS3 to work with EXOS-VM.  If you have any questions about this guide please open a [Issue](https://github.com/extremenetworks/Virtual_EXOS/issues/new) on GitHub or on  [The HUB](http://community.extremenetworks.com/).  

**Note: EXOS-VM's can get stuck in (pending AAA) for 1-2 minutes.  Just be patient it will finish, and allow you to login**.

### What you will need:
* Vmware player - latest version  --  ```This is needed for the GNS3-VM```
 	* https://www.vmware.com/products/player
 	
* VMware VIX API - latest version -- ```You need this so GNS3 can control Vmware player```
	* 	* https://www.vmware.com/support/developer/vix-api/
	
* GNS3-VM.ova from GitHub  --  ```This version must match the version of GMS3 on your local machine```
 	* GNS3-VM.ova
 		*  https://github.com/GNS3/gns3-vm/releases

* GNS3 for your local machine.  -- ```This version must match the version of GNS3-VM``` 
 	*  GNS3-X.X.X-all-in-one.exe
 		*  https://www.gns3.com/software/download

* GNS3 Template File for EXOS VM  -- ```This is used to import EXOS into GNS3```
	* exosvm.gns3a
		* https://github.com/extremenetworks/Virtual_EXOS/blob/master/exosvm.gns3a?raw=true

------
### Getting Started:

#### Step 1: Download GNS3 Template File
* Download GNS3 Template File for EXOS VM.  --  ```You will need this in Step 8```
	* https://github.com/extremenetworks/Virtual_EXOS/blob/master/exosvm.gns3a?raw=true

#### Step 2: Vmware player

* Download and install Vmware player. 

#### Step 3: VMware VIX API

* Download and install VMware VIX API

#### Step 4: GNS3-VM.ova
1.  Download GNS3-VM.ova from GitHub  -- ```This version must match the version of GMS3 program on your local machine```
2.  Import the GNS3-VM.ova into Vmware player.  **Don't start it yet.**
3.  Edit the VM to make sure you give it as much memory and CPU's as you can.  This will help improve your experience when using GNS3 and EXOS-VM.  I recommend giving the VM all CPU's and half of your RAM.

#### Step 5: GNS3 for your local machine
* Download and install GNS3 program for your local machine.  -- ```This version must match the version of GNS3-VM```

#### Step 6: Open GNS3
1.  Make sure Vmware player is open but **NOT** booted up.
2.  Open GNS3

#### Step 7: Setting up GNS3
1. A Setup Wizard should show up when you open GNS3.  Select "Local GNS3 VM" and click next.  
2. Click on "VMware" -> Select your GNS3-VM -> and select the same CPU's and RAM you picked in Step 4.3. -> Click Next
3. Your GNS3-VM should now start booting up.  Wait for it to boot, and uncheck all boxes and click finish on the GNS3 wizard.
4. Close the Preferences window -> Continue without saving -> Yes -> Name your Project, and click OK.

#### Step 8: Import EXOS-VM as Appliance 
1. Go to File -> Import appliance -> Open the exosvm.gns3a file downloaded in Step 1.
2. Click next -> Select "Run the appliance on the GNS3-VM" -> Click next.
3. You should see two versions of EXOS.  Expand the version you want and click on the file. -> click download.
4. Once downloaded Click on import, and select the file you just downloaded. -> Click Next -> Click Yes -> Click Next -> Click Finish -> Click OK.
5. Now you will see a router that is called "EXOS VM XX.X.X.X" in your inventory.
6. Drag the VM to your project. and select yes to upload your image to your VM.

### Step 9: Have fun!
1. Move more switches over connect them together, boot them up, and configure them.  Be careful for loops!
