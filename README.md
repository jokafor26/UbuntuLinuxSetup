# UbuntuLinuxSetup

Ubuntu Linux Virtual Machine Setup

I installed the hypervisor VirtualBox from the virtual box website. I also got the iso file I’ll be using to install on the Virtual box which was Ubuntu 64-bit version 16.04.3.

I installed Ubuntu operating system twice on virtual box, so I had 2 virtual machines with Linux software.

 <img width="223" height="211" alt="Image" src="https://github.com/user-attachments/assets/8d72ddab-5fd6-46c9-8a21-dfbf4c803911" />

Trying to ping the machines I ran into multiple errors, and roadblocks. At first, I couldn't ping the host OS let alone another virtual machine. Some of these issues involved firewall of the host OS, the network adapter not being found in my guest OS, my VirtualBox not having the packages which allow my virtual machines to use the host adapter.
I installed the packages which was called Oracle VM VirtualBox Extension Pack. I proceeded to try to ping my host OS but still failed. I realized I had an Ip address of 10.0.2.5 which granted me internet access. I changed it to a different Ip address, but then I couldn't get access to the internet or ping any sites or Ips. I turned off the virtual machine and switched the network interface from NAT to bridge which did not end up working. I did some reading I found out I had to use a host only adapter setting for my virtual machine to get in contact with my host. This ended up working, but I couldn't get access to the internet. This is because Host-only lets me connect to the host because there is a private internal network between them, but cannot give it internet access with the virtual machine which only the Host could. So, I had to add another adapter to my virtual machine which ended up being NAT, because the NAT setting allows my virtual machines to connect to the internet (In the beginning I had internet access with NAT settings before switching to Bridge).
	With all these settings corrected the only problem among me trying to access the host, and get internet access through the host was that my Firewall of my host OS prevented me from sharing network or being found. I turned it off, and tested if I could ping and virtual machine, host machine and browse the internet. I got the Ip of my host and 2 virtual machines, and pinged it. I got results for all: pinging the host for a virtual machine, pinging a virtual machine from the host, and getting internet access with the virtual machines.

<img width="463" height="349" alt="Image" src="https://github.com/user-attachments/assets/984b1d6d-3cbb-4d96-b5dd-8d35c3116201" />
 
<img width="418" height="276" alt="Image" src="https://github.com/user-attachments/assets/6c1cc684-fb25-468c-aaa3-3e6d1b8c9725" />
 
 <img width="599" height="595" alt="Image" src="https://github.com/user-attachments/assets/5dd49d0a-f4b3-4fd7-83ad-4c2e6affef95" />
 
<img width="780" height="569" alt="Image" src="https://github.com/user-attachments/assets/ef49bdba-e464-40e2-8e5e-6238c07ee7d7" />

<img width="718" height="273" alt="Image" src="https://github.com/user-attachments/assets/5606aa69-836d-40bd-a342-3e56916ece12" />

<img width="655" height="388" alt="Image" src="https://github.com/user-attachments/assets/2fbb2bac-3472-45b4-8280-51701edb6ec8" />

<img width="1317" height="697" alt="Image" src="https://github.com/user-attachments/assets/e84a180f-0c1e-411e-b352-fc4225c08eff" />








 
