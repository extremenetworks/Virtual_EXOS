EXOS-VM Requirements for VMware ESXi

To deploy an EXOS-VM on VMware ESXi, use the configuration settings outlined below. After creating the virtual machine, mount the EXOS-VM ISO via the CD-ROM drive and boot the VM to install the image. Once the installation is complete, unmount the ISO.

   Note: EXOS-VMs may appear stuck at "(pending AAA)" for 1–2 minutes during boot. This is expected—please be patient and wait for the login prompt to appear.

Recommended ESXi VM Configuration for EXOS-VM

   Guest OS: Other Linux (64-bit)

   Virtual CPUs:

   Sockets: 1

   Cores per Socket: 2

   Memory (RAM): 512 MB

   Hard Drive:

  - Size: 4 GB

      Controller: SCSI (LSI Logic Parallel)

       Provisioning: Thick Provisioned

      IDE (0:0): Required for proper boot configuration

    CD-ROM Drive: Required for mounting the EXOS-VM ISO during installation

Network Interface Mapping

   NIC 1: Management Interface
   NICs 2–14: Data Interfaces (up to 13 supported)
