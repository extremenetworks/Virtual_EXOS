# Importing and Exporting individual GNS3 projects on GNS3-VM

A EXOS GNS3 project consist of three things.  On your PC you have a screenshot.png file and a .gns3 file.  On your GNS3-VM there is a Project folder in the "/opt/gns3/projects" directory on the VM.

> Finding which project folder in the GNS3-VM is linked to a project is easy.  Open the .gns3 file in notepad, the 4th line of the file will tell you the project ID.  This project ID will be the same as the folder name in the "/opt/gns3/projects" directory.



## Exporting individual projects
When exporting your project you need to gather the files already on your PC and download your project folder on the GNS3-VM.  I recommend keeping your local PC files where they are, and just download your GNS3-VM project folder to the same folder as you’re .gns3 file.

##### Step 1:
Locate your GNS3 project on your PC.  On a PC it's usually located here "\%userprofile%\gns3\projects".

##### Step 2:
Open the .gns3 file in notepad, and locate the project ID.  This will be the same as your folder name in your GNS3-VM.  Remember this project ID for step 4

##### Step 3:
Use an ftp program to connect to your VM.
>Note: The IP of the VM should show up on the VM and the **username/password is gns3/gns3**

##### Step 4:
Now that your connected, go to "/opt/gns3/projects" and download the folder that matches your project ID.

**I then like to ZIP the entire project for safe keeping.**


## Importing individual projects:

All projects should contain a project folder like this "6d938f08-fd90-4e7f-ad47-5821080b46d2" and at least a .gns3 file.


##### Step 1:
Boot up GNS3 and your GNS3-VM.

##### Step 2:
Use an ftp program to connect to your VM.
>Note: The IP of the VM should show up on the VM and the **username/Password is gns3/gns3**

##### Step 3:
Now that your connected, go to "/opt/gns3/projects" and upload the project folder to this location.

> Note the Project folder will look something like this "6d938f08-fd90-4e7f-ad47-5821080b46d2"

##### Step 4:

open the .gns3 project file in GNS3.
