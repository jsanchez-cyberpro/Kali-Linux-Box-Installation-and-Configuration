## Kali Linux - Installation and Configuration

The steps in this repository were used to Download and install VirtualBox along with Kali Linux.
 
This document contains the following details:
- Download Link to VirtualBox 
- Download Link to Kali Linux 
- Installation Instruction for VirtualBox
- Configure Kali Linux


### Download and Install VirtualBox 

VirtualBox is a powerful virtualization software that allows users and administrators to easily run multiple guest operating systems on a
single host. In our case we are going to use VirtualBox enviroment for testing and learning tool. 

With the help of a VirtualBox, you can install Kali Linux in your system (in a seperate enviroment) from your primary OS.

Let's walk through how to Download and install a VirtualBox enviroment in your computer. 

Step 1 - To Download, go to https://www.virtualbox.org/wiki/Downloads. Depending on your host OS, select the right package. In this case,
it will be the first package for windows hosts shown in the following screenshot. 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/Download_page_screenshot.JPG)


Step 2 - Open the Dowloaded .exe file and click next

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/VirtualBox%202.JPG)


Step 3 - The next page will give you an option to choose the location where you wan to install the application. In this case, let us leave it as default
and click Next. 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/VirtualBox%203.JPG)


Step 4 - Click Next and the following Custom Setup screenshot pops up. Select the features you want to installed and click Next. 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/Virtual%20Box%204.JPG)


Step 5 - Click Yes to begin with the installation. 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/Virtual%20Box%205.JPG)


Step 6 - The Ready to Install screen will pop up next. Click Install. 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/Virtual%20Box%206.JPG)


Step 7 - Click the finish button 

![alt text](https://github.com/jsanchez-cyberpro/Kali-Linux-Box-Installation-and-Configuration/blob/main/Dowload%20and%20Install%20Virtual%20Box/Virtual%20Box%207.JPG)


### Install Kali Linux 

Once the VirtualBox Application is done installing. The application windows will open as shown in the following screenshot. Now you're ready to move forward
with the installation of the Kali Linux OS. 

Step 1 - Download the Kali Linux package from its offical site https://www.kali.org/downloads/
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Diagrams/Virtual_Network_Map.JPG)

Step 2 - Open VirtualBox --> under Machine select --> New as shown in the screenshot below. 
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Diagrams/Virtual_Network_Map.JPG)

Step 3 - Choose the right Virtual Hard Disk File and click Open.
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Diagrams/Virtual_Network_Map.JPG)

Step 4 - Under the Create Virtual Machine Screen click on Create.
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Diagrams/Virtual_Network_Map.JPG)

Step 5 - Start Kali Box. The default username is root and the password is toor.
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Diagrams/Virtual_Network_Map.JPG)

### Configure and Update Kali  

It is vital to update Kali Linux and its tool to the new versions after installation. We are also going to perform some administrative changes
to ensure our box is as secure as possible. Please Follow the steps below:

Step 1 - Making sure Kali is Up to Date. First Open the Terminal in Kali and run: sudo apt update && sudo apt dist-upgrade -y 

![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Ansible/docker_ps_screenshot.png)
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Ansible/docker_ps_screenshot.png)

Step 2 - Changing the default password type: passwrd --> then it will prompt you for the current password. Type toor and then your new password
and go ahead and confirm the new password by retyping it. 

![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Ansible/docker_ps_screenshot.png)

Step 3 - Creating a Low Privileged User Account.Type --> Sudo adduser Username, enter the password but make sure its different than the root password.
This will create a new user as well as a home folder. To verify a home folder was created type --> ls /home/  

![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Ansible/docker_ps_screenshot.png)

Step 4 - Remove the new user just created from Sudo group. This will ensure even if your account is compromised, the attack will not have sudo privilages
unless they managed to also compromise the 'root' account. This will provide an extra layer of protection. 
  
![alt text](https://github.com/cyberprotocols/cyberpro_inc/blob/main/Ansible/docker_ps_screenshot.png)


### Educate yourself!

Now that you have been fulle equiped with the right technical set up, it's time to upgrade yourself. I will be posting more How-To on Installing useful tools
for Ethecial Hacking. 

##Subdomain Enumeration

- Amass
- Subfinder
- AssetFinder
- Ffuf
- Gowitness

##Directory Bruteforcing

- FFuf
- Turbo Intruder
- GoBuster
- Dirsearch

##General Tools

- Metasploit
- Hydra
- JohnTheRipper
- KeepassXC
- Cherrytree
- Searchsploit
