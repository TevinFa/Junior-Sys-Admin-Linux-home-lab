# Junior-Sys-Admin-Linux-home-lab
Purpose: Building and maintaining an Ubuntu Linux environment including user administration, server configuration, SSH hardening, performance monitoring and log analysis. 

Step 1: Install Ubuntu ISO image 

Installed from [https://ubuntu.com/download/server]

<img width="1255" height="805" alt="image" src="https://github.com/user-attachments/assets/dfac4397-8b9b-4652-a62b-08ed3d2955bc" />

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

Step 5: Write a script to create users. (My users will be sports users because I am a sports fan)

Opened terminal and created a new file with touch command and gave it the name create_sports_users.sh

<img width="301" height="28" alt="image" src="https://github.com/user-attachments/assets/fb31afc6-ca88-4c2e-9f69-0702105f6cf2" />

Opened the file using the Nano text editor. 

<img width="290" height="23" alt="image" src="https://github.com/user-attachments/assets/7acb826a-adf8-473a-9ec6-ac85e0be8e67" />

Wrote the code to create nbaplayers 1-5, mlbplayers 1-5 and nflplayers 1-5 and then save the file. 

<img width="599" height="365" alt="image" src="https://github.com/user-attachments/assets/7217914c-16c2-48c9-82e2-f53c5af4f845" />

Make the file executable. 

<img width="353" height="53" alt="image" src="https://github.com/user-attachments/assets/7112d29e-e88f-434e-a2f9-0685023a6dcd" />

Run the script to create the users. 


<img width="226" height="47" alt="image" src="https://github.com/user-attachments/assets/9c289a58-fa7f-45d8-a5af-38d59575bf36" />




<img width="568" height="528" alt="image" src="https://github.com/user-attachments/assets/6dd25927-3164-4e63-a889-7f38aa9ae721" />




<img width="567" height="339" alt="image" src="https://github.com/user-attachments/assets/1bcb7167-8280-4ce7-a556-eb905d4da098" />






