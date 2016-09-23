# Importing and Exporting individual GNS3 projects on GNS3-VM 1.5.2 and above.

GNS3 V1.5.2 has made it very easy to import and export GNS3 project.

## Exporting individual projects:

##### Step 1:
Open the project

##### Step 2:
Click file, and then Export

![](import_export.jpg "Export")

##### Step 3:
You will be given the option to include the base image.  The base image is the .qcow2 EXOS images.  If you select yes, you will download one 117MB image for each switch in your project.  This will make you backup very large.  If you select "No" everything will be backuped except the images.  Your switch configurations AKA "QEMU snapshots", and network connections will be backed up.

![](image_YN.jpg "Base Image Yes/No")

## Importing individual projects:

##### Step 1:
Open GNS3

##### Step 2:
Click file, and then Import

![](import_export.jpg "Import")

##### Step 3:
Select your project and click open.

> Note: If the project uses a specific .qcow2 EXOS image you will need to have the Device/version added into GNS3 Devices section.  See [GNS3 with EXOS-VM install Guide](https://github.com/extremenetworks/Virtual_EXOS/blob/master/GNS3_EXOS-VM_Guide.md) for steps.

##### Step 3:
Start your switches and Enjoy!



> Backup files are just .zip files and can be extracted to see contents. 
