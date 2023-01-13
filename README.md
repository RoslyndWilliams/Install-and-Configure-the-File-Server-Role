<p align="center">
<img src="https://i.imgur.com/4wqxHID.png" height="40%" width="60%" alt="Microsoft Azure Logo"/>
</p>

<h1>Microsoft Server</h1>
Imagine this scenario: you are using the CorpFiles16 server as a file server. You can do basic file server management for network users, but you need to be able to perform the following file server management tasks:

- Define policies that prevent users from saving .wmv files in the home folders stored on the server.
- Share files with UNIX-based clients.

In this scenario, your task is to perform the following:

- Add the File Server Resource Manager (FSRM) role service, which allows you to configure file screens to prevent users from saving specific file types in specific folders.
- Add the Server for NFS role service to be able to share files with UNIX-based clients.




<h2>Requirements</h2>

- Computer with Internet Connection
- Credit Card (Required for free Azure credits)

<h2>Configuration Steps</h2>


<h3>Step 1: Create an Azure Account</h3>


Create an Azure account [here](https://azure.microsoft.com/en-us/free/).
- Select Start Free
- Follow the prompt to create the account 
     - You will need to put in your credit card information, but you will get $200 worth of Azure credit and will have 30 days to use those credits. You will not be charged until then
- Finish the prompt, click Go to Azure Portal, and you are ready to start with Azure!
     - You may also go to [portal.azure.com](https://www.portal.azure.com) to start


<p align="center">
<img src="https://i.imgur.com/rk4SD27.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/f1eRIx4.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 2: Create a Resource Group</h3>

- Go to the search bar at the top and search "resource group"
- Select Create Resource Group
- You will need to name the resource group and select the region 
- Select Review + Create on the lower left
    - For this example, we will be using RG-Lab-1 for the name and (US) West 3 for the region

<p align="center">
<img src="https://i.imgur.com/Afnk87u.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/yBBln5a.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>

<h3>Step 3: Create a Storage Account</h3>

- Go to the search bar and search "storage account"
- Select Create Storage Account
- You will need to select the same resource group, the same region, and create a name for the storage group
    - For this example, we will name the storage group "rglab1"
    - Use the same resource group and region as step 2
- Select Review, then Create

<p align="center">
<img src="https://i.imgur.com/zhb3GHZ.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/7ryNBQg.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 4: Create a Virtual Machine</h3>
     
- Go to the search bar and search "virtual machine"
- Select Create, then select Azure Virtual Machine
- You will need to select the same resource group, the same region, and create a name for the virtual machine
    - For thise example, we will name the virtual machine "virtualmachine"
    - Use the same resource group and region as steps 2 and 3

<p align="center">
<img src="https://i.imgur.com/y0RafHM.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/PCJ3QAr.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>
 



* You will then need to select the image and disk size
    - For image we will use Windows 10 Pro
    - For size, select See All Sizes and select Standard D2as_v4
* You will then need to make a username and password
    - For username, we will use "labuser"
    - Create your own password
* Click the box under licensing and finally click Review + Create 


<p align="center">
<img src="https://i.imgur.com/p9UJXND.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/GHBDae0.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>
 
     

<h3>Step 5: Connect to the Virtual Machine</h3>

- First, you will need to find the public IP address of your virtual machine
   - Select the virtual machine we created and the public IP address will be on the right-hand side of the screen
   - Copy the public IP address

<p align="center">
<img src="https://i.imgur.com/T4Oc2RX.png" height="80%" width="80%" alt="Azure Free Account"/>

* Mac Users 
   - Download Microsoft Remote Desktop
   - Open the application and click Add PC
   - Paste the public IP address and select Add
   - Double-click on the virtual machine and enter the username and password from step 4
   - Select Continue
   
* Windows Users
     - Open and use Remote Desktop
     - Paste the public IP Address and select Connect
     - Enter the username and password from step 4
     - Select OK
  
     
     
 <p align="center">
<img src="https://i.imgur.com/14pPOdv.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/Og3LKyd.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>





🎉Congratulations! You have created your first virtual machine within Azure!🎉

<p align="center">
<img src="https://i.imgur.com/rEBpL8Y.png" height="80%" width="80%" alt="Azure Free Account"/>

<h3>Tip</h3>

-  In case you need to restart the server after finishing the installation, check the box on the Confirmation screen that says "Restart the destination server automatically if required." As a warning, the server will restart after isntallation without further warning, so ensure no files or services are being remotely accessed at the tim eof the restart, otherwise the person working on th eremote file will lose server connectivity--and possibly lose any cahgnes they made to the document.
 
