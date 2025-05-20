# BGP with route redistribution to and from OSPF

This GNS3 project was made to show a configuration example of BGP.  There are three separate BGP ASes, and two OSPF ASes.

Note: These projects were built for the EXOS-VM_v32.7 images.  Make sure the image is loaded into GNS3 before you import the project.

* [GNS3 32.7 Project file](https://github.com/stewilliams-extr/Virtual_EXOS/raw/refs/heads/master/gns3_projects/BGP/BGP_32.7.2.gns3project)

* [Configuration Files and Routing Tables](configs)
  
<img src="screenshot.png">

* [How To: Troubleshoot BGP Issues on Switch Engine (EXOS)](https://extreme-networks.my.site.com/ExtrArticleDetail?an=000078327)
* 
>Note: ECMP is not supported in EXOS-VM. This is because ECMP requires hardware support, and the required hardware is not emulated in the VM.
