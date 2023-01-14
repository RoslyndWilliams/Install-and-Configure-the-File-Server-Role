<p align="center">
<a href="https://imgur.com/xs8Rs9B"><img src="https://i.imgur.com/xs8Rs9B.png" title="source: imgur.com" height="40%" width="60%" /></a> 
</p>

<h1>Windows Server</h1>
Imagine this scenario: you are using the CorpFiles16 server as a file server. You can do basic file server management for network users, but you need to be able to perform the following file server management tasks:

- Define policies that prevent users from saving .wmv files in the home folders stored on the server.
- Share files with UNIX-based clients.

In this walkthrough, we'll perform the following file server management tasks

- Add the File Server Resource Manager (FSRM) role service, which allows you to configure file screens to prevent users from saving specific file types in a specific folder
- Add the Server for NFS role service to be able to share files with UNIX-based clients.


<h2>Environments and Technologies Used</h2>

- Computer with Internet Connection
- Microsoft Azure
- Microsoft virtual machine
- Microsoft Windows Server 2012 Datacenter 

<h2>Program Walk-Through:</h2>



<h3>Launch Server Manager and Hyper-V Manager</h3>

<p align="center">
<a href="https://imgur.com/yXFOgcw"><img src="https://i.imgur.com/yXFOgcw.png" title="source: imgur.com" height="70%" width="70%" alt="Step 1- Launch Server Manager Hyper-V Manager" /></a>
</p>


<h3>Switch to the CorpFiles16 Server</h3>

<p align="center">
<a href="https://imgur.com/ljHW2r6"><img src="https://i.imgur.com/ljHW2r6.png" title="source: imgur.com"  height="70%" width="70%" alt="Step 2- Switch to the CorpFiles16 Server" /></a>
</p>


<h3>Observe System Name to Confirm System is Switched to CorpFiles16 Server</h3>

<p align="center">
<a href="https://imgur.com/wj0gOJ3"><img src="https://i.imgur.com/wj0gOJ3.png" title="source: imgur.com" height="70%" width="70%" alt="Step 3- Observe System Name to Confirm System is Switched to CorpFiles16 Server" /></a>
</p>


<h3>Open the Add Roles and Features Wizard</h3>

<p align="center">
<a href="https://imgur.com/OGQvuGw"><img src="https://i.imgur.com/OGQvuGw.png" title="source: imgur.com"  height="70%" width="70%" alt="Step 4- Open the Add Roles and Features Wizard" /></a>
</p>


<h3>Move Through Various Steps to Access Server Roles tab
     <p>Expand and Choose FSRM</p></h3>

<p align="center">
<a href="https://imgur.com/Nn6CbR9"><img src="https://i.imgur.com/Nn6CbR9.png" title="source: imgur.com" height="80%" width="80%" alt="Step 5- Move Through the Various Steps to Access the Server Roles tab, then Expand and Choose FSRM" /></a>
</p>


<h3>Add Required Features for FSRM</h3>

<p align="center">
<a href="https://imgur.com/0AWvlx2"><img src="https://i.imgur.com/0AWvlx2.png" title="source: imgur.com" height="80%" width="80%" alt="Step 6- Add Required Features for FSRM" /></a>
</p>


<h3>Select NFS Role</h3>

<p align="center">
<a href="https://imgur.com/ES7Mn1U"><img src="https://i.imgur.com/ES7Mn1U.png" title="source: imgur.com" height="80%" width="80%" alt="Step 7- Select NFS Role" /></a>
</p>


<h3>Add Required Features for NFS</h3>

<p align="center">
<a href="https://imgur.com/lgVoFTd"><img src="https://i.imgur.com/lgVoFTd.png" title="source: imgur.com" height="80%" width="80%" alt="Step 8- Add Required Features for NFS" /></a>
</p>


<h3>Confirmation Page</h3>

<p align="center">
<a href="https://imgur.com/fek87gj"><img src="https://i.imgur.com/fek87gj.png" title="source: imgur.com" height="80%" width="80%" alt="Step 9- Confirmation Page" /></a>
</p>


<h3>Installation Confirmed</h3>

<p align="center">
<a href="https://imgur.com/vsy96lq"><img src="https://i.imgur.com/vsy96lq.png" title="source: imgur.com" height="80%" width="80%" alt="Step 10- Installation Confirmed" /></a>
</p>
