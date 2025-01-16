# Vitual Private Network (VPN)
<p align="center">
<img src="https://i.imgur.com/MntON5Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation ousing a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating IP Through VM (France)
- STEP 4 - Connecting to VPN Through VM
- STEP 5 - Locating IP Through VPN (Japan)

<h2>Installation Steps</h2>

First, locate your own personal IP address by going to "www.whatismyipaddress.com" which will be able to show you your local IP address. We will use this later as well.
<p>
<img src="https://i.imgur.com/pKmIEeu.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will set up a virtual machine on Azure. 
  
</p>
<br />

Go to www.portal.azure.com and find Virtual Machines. Create a VM with Windows 10 as the image. For the region, I typically create the VM in (US) West US.

<p>
<img src="https://i.imgur.com/BQOR7Bm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/iCBdIqw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


For the Username and Password you can create your custom information, just record it personally.
<p>
Before you review+create, make sure the licensing box is checked.
</p>
<br />

<p>
<img src="https://i.imgur.com/KXb9B9h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/INleKv1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

After the VM is created, open remote desktop, and log into your VM using the public IP Address.
<p>
<img src="https://i.imgur.com/fjxAVaU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When we look up the IP address for this VM through www.whatismyipaddress.com we see that this VM is showing the location for Washington, US (EXAMPLE 3C).
<p>
<img src="https://i.imgur.com/kwxeQj9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now head over to ProtonVPN and sign up for a free account.  
</p>
<img src="https://i.imgur.com/pbxWJAI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. See EXAMPLE 4B when this steps are completed.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in Japan. See EXAMPLE 4C
  
</p>
<br />

EXAMPLE 4C
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to Japan. The website www.whatismyipaddress.com shows yet another IP address using the VPN from Japan. This is quite amazing.
  
</p>
<br />

EXAMPLE 4D
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 137.103.51.136
Virtual Machin IP (France): 20.216.176.18
Virtual Machin IP VPN (Japan) 212.102.51.251

  
</p>
<br />
If you no longer need the VM, ensure to remove it from the Asure account for unwanted charges.

END OF TUTORIAL
