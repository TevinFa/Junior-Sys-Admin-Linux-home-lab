<DOCTYPE HTML>

  
# Junior-Sys-Admin-Linux-home-lab
Purpose: Building and maintaining an Ubuntu Linux environment including user administration, server configuration, SSH hardening, performance monitoring and log analysis. 
<DOCTYPE HTML> 

Step 1: Install Ubuntu ISO image 

Installed from [https://ubuntu.com/download/server]
<h1>Junior-Sys-Admin-Linux-home-lab</h1>

<img width="1255" height="805" alt="image" src="https://github.com/user-attachments/assets/dfac4397-8b9b-4652-a62b-08ed3d2955bc" />
<p>Purpose: Building and maintaining an Ubuntu Linux environment including user administration, server configuration, SSH hardening, performance monitoring and log analysis.</p>

Step 2: Setup Virtual Machine using Ubuntu ISO image

<img width="708" height="403" alt="Create_New_Virtual_Machine" src="https://github.com/user-attachments/assets/9cfea7e8-84e4-445f-8c0c-4436610b68fc" />

Next set a username, password and hostname. I checked Guest Additions for additional functionality among my VM and host machine.

<img width="707" height="400" alt="image" src="https://github.com/user-attachments/assets/7dc8cdb5-977a-4589-a1e0-f718374a9a32" />

Set Base Memory to 4096 MB and 2 Processors.

<img width="710" height="405" alt="image" src="https://github.com/user-attachments/assets/b8934eb0-3f17-4d39-ad46-28d67b456b11" />

Set Virtual Hard Disk to 50 GB to give myself a good amount of storage space. The Ubuntu operating system will need at least 20 GB of storage. 

<img width="718" height="407" alt="image" src="https://github.com/user-attachments/assets/28783449-a865-49cf-8920-c4a95719182c" />

Enabled Shared Clipboard under general settings so that I can copy and paste between my host machine and VM. Under network settings, set the network adapter to bridged adapter and pointed it to my wifi adapter so that my vm can run off my host network and I want to be able to ssh into my server from other devices connected on the same network. 

<img width="625" height="487" alt="image" src="https://github.com/user-attachments/assets/d1984639-1f7b-4d9c-9bcc-a1785d84573c" />

Step 3: Update/Upgrade Packages 

Opened a terminal window, switched to root and ran apt update and apt upgrade commands. (No upgrades because I already upgraded prior to creating this documentation)

<img width="716" height="177" alt="image" src="https://github.com/user-attachments/assets/3677be09-cc7f-4526-ade2-217c77b0427c" />

<img width="581" height="112" alt="image" src="https://github.com/user-attachments/assets/f7514706-90c3-4b3b-a550-162bb82bd22b" /> 

Step 4: Create a Snapshot (in case something breaks)

Click Machine > Take Snapshot

<img width="578" height="174" alt="image" src="https://github.com/user-attachments/assets/23829fa3-e335-49c6-8924-a91831cabcd4" />

Step 5: Add 2 new users

<img width="421" height="24" alt="image" src="https://github.com/user-attachments/assets/0f000ddd-5bd2-466f-8792-bc7e6d9fbec1" />

<img width="403" height="30" alt="image" src="https://github.com/user-attachments/assets/1453bf57-9175-4032-bfdd-21ad42569ddd" />

Step 6: Create group helpdesk and append user1 and user2 to the helpdesk group

<img width="475" height="38" alt="image" src="https://github.com/user-attachments/assets/f4abd8e7-3c1f-4f05-84cd-6d19626e01e8" />

<img width="491" height="24" alt="image" src="https://github.com/user-attachments/assets/c762f6a8-0f0d-44db-b57d-0bf56811b0da" />

Step 7: Create a directory named shared, give read, write and execute permissions to the owner and helpdesk group. 

<img width="405" height="26" alt="image" src="https://github.com/user-attachments/assets/0c316519-167b-4a5f-8a23-dd880e19d34f" />

<img width="483" height="29" alt="image" src="https://github.com/user-attachments/assets/fb04f748-5117-43bb-abb6-f030f8989d39" />

<img width="431" height="26" alt="image" src="https://github.com/user-attachments/assets/60695b0e-3d71-4e1d-b825-15a1cde8e6d4" />

Step 8: Install Apache2 web server and confirm successful installation by navigating to http://localhost in the browser. 

<img width="463" height="27" alt="image" src="https://github.com/user-attachments/assets/f8831fd5-52bb-4e58-a2b4-be237aaa4afc" />

<img width="981" height="738" alt="image" src="https://github.com/user-attachments/assets/87ea122e-c7ac-4474-85b7-803b7732a058" />

















