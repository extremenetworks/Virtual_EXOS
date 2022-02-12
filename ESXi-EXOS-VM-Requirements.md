# ESXI requirements for EXOS-VM
When building a EXOS-VM in ESXI use the below ESXI VM settings to build the VM.  Once the VM is built attach the CDROM with the EXOS-VM ISOs and boot up the VM to install the Image.  Once installed remove the ISO from the VM.  The first NIC is the Mgmt port, and the other ports up to 13 more are data ports.


**Note:   EXOS-VMs can get stuck in (pending AAA) for 1-2 minutes.  Just be patient it will finish, and allow you to login**.

### ESXI EXOS-VM settings
* Guest OS: Other Linux 64-bit
* Virtural Sockets: 1
* Cores per Socket: 2
* Ram: 512MB
* Hard Drive space: 4GB
* Hard Disk:
 	* SCSI - LSI Login Parallel
 	* Thick Provision
 	* IDE(0:0) - required.
 	* Mode Dependent
 	* CDROM: for EXOS-VM ISO
