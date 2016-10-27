# OSPFv3 Area example GNS3 project

This GNS3 project was made to show a configuration example of how different OSPFv3 area types are configured using IPv6.  In the picture below you can see that each area shows a example of a different way to use a OSPF area.

Note: This project was built with the EXOS-VM_v21.1.1.4-disk1.qcow2 image.  Make sure you the image is loaded into GNS3.

* [GNS3 Project file](https://github.com/extremenetworks/Virtual_EXOS/blob/master/gns3_projects/OSPFv3_areas/ospfv3.gns3project?raw=true)

* [Configuration Files](configurations)

<img src="screenshot.png">
>Note: in this example /24 networks are used as P2P links.  You would normaly use /30 for P2P links.  I wanted to make the last Octet of the IP to reflect the Switch #.
OSPFv3_areas
