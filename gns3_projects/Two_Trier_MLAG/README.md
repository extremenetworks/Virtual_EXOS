# Two tier MLAG example GNS3 project

This GNS3 project was made to show a configuration example of how Two tier MLAG is configured.  Vlan Data is across all switches.

Note:These projects were built for the EXOS-VM_v32.7-disk1.qcow2.  Make sure the image is loaded into GNS3 before you import the project.

* [GNS3 32.7 Project file](https://github.com/stewilliams-extr/Virtual_EXOS/blob/master/gns3_projects/two_tier_MLAG/MLAG.gns3project)
* [Configuration Files](configurations)

<img src="screenshot.png">

>Note: The MLAG failover may take up to 10 sec becasue of limitations with GNS3 and qemu devices.  LLDP was used to allow failover to happen.
