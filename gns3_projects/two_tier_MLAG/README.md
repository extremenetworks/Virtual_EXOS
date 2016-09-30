# Two tier MLAG example GNS3 project

This GNS3 project was made to show a configuration example of how Two tier MLAG is configured.  Vlan Data is across all switches.

Note: This project was built with the EXOS-VM_v21.1.1.4-disk1.qcow2 image.  Make sure you the image is loaded into GNS3.

* [GNS3 Project file](https://github.com/extremenetworks/Virtual_EXOS/blob/master/gns3_projects/two_tier_MLAG/MLAG.gns3project?raw=true)
* [Configuration Files](configurations)

<img src="screenshot.png">

>Note: The MLAG failover may take up to 2-3 minutes becasue of limitations with GNS3 and qemu devices.  LLDP was used to allow failover to happen.
