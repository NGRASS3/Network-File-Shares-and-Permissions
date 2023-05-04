![image](https://user-images.githubusercontent.com/111653930/236330155-0a4f433f-f22d-4af6-a88e-3e192dc9a261.png)


<h1>Network-File-Shares-and-Permissions</h1>
In this tutorial were going to be sharing out files and folders over the Network and allowing different people and groups different levels of access.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Domain Controller/Client Machine)
- Remote Desktops with Active Directory
- Shared Network Files

<h2>Operating Systems Used </h2>

- Windows 10(21H2)

<p>
To start we will login to our Domain Controller DC-1 as an admin account, and our Client-1 as a normal user. Inside DC-1 we will create 4 new folders on the C:\ drive. 
  
  1. Read-Access
  2. Write-Access
  3. No-Access
  4. Accounting
</p>

![image](https://user-images.githubusercontent.com/111653930/236332672-05b594de-e8d5-469e-81d9-f6d3ce785c3e.png)

<p>
We will now set the following permissions for the "Domain Users" group:
  
 - Folder: read-access, Group: Domain Users, Permission: Read
 - Folder: write-access, Group: Domain Users, Permission: Read/Write
 - Folder: no-access, Group: Domain Admins, Permission: Read/Write
  
  
  In order to set these permissions navigate to the file (read-access in this example) -> right click Properties -> Sharing -> and add the appropriate parameters based on the list above.
  
</p>

![image](https://user-images.githubusercontent.com/111653930/236337087-3eda95d0-e849-41af-972e-9904ad1c13fc.png)
![image](https://user-images.githubusercontent.com/111653930/236337103-b5ecc273-7d36-4c75-832e-5e8eecf7723e.png)
![image](https://user-images.githubusercontent.com/111653930/236337134-8b87996b-fd48-4bf4-989c-82d350915f99.png)



