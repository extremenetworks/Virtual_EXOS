# OSPF Area example GNS3 project

This GNS3 project was made to show a configuration example of how different OSPF area types are configured.  In the picture below you can see that each area shows a example of a different way to use a OSPF area.

Note: These projects where built for the EXOS-VM_v21.1.1.4-disk1.qcow2 and the EXOS-VM_v22.1.1.5-disk1.qcow2 images.  Make sure the image is loaded into GNS3 before you import the project.

* [GNS3 21.1 Project file](https://github.com/extremenetworks/Virtual_EXOS/blob/master/gns3_projects/OSPF_areas/ospfv2.gns3project?raw=true)
* [GNS3 22.1 Project file](https://github.com/extremenetworks/Virtual_EXOS/blob/master/gns3_projects/OSPF_areas/ospfv2.gns3project?raw=true)
* [Configuration Files](configurations)

<img src="screenshot.png">
>Note: in this example /24 networks are used as P2P links.  You would normaly use /30 for P2P links.  I wanted to make the last Octet of the IP to reflect the Switch #.
