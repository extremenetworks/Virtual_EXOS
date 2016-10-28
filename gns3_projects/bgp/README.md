# BGP with route redistribution to and from OSPF

This GNS3 project was made to show a configuration example of BGP.  There are three separate BGP ASes, and two OSPF ASes.

Note: This project was built with the EXOS-VM_v21.1.1.4-disk1.qcow2 image.  Make sure the image is loaded into GNS3.

* [GNS3 Project file](https://github.com/extremenetworks/Virtual_EXOS/blob/master/gns3_projects/bgp/bgp.gns3project?raw=true)
* [Configuration Files and Routing Tables](configurations)

<img src="screenshot.png">

>Note: ECMP is not supported in EXOS-VM. This is because ECMP requires hardware support, and the required hardware is not emulated in the VM.
