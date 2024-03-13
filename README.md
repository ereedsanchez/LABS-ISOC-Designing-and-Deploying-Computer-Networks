# LABS-ISOC-Designing-and-Deploying-Computer-Networks

## Lab 1 - 
#### Lecture: https://docs.google.com/presentation/d/1-A1YdEBYIDAOlrksCNzp31u37SOQqAPIBkinkNxtqNY/edit?usp=sharing
- Course Background
- Introductions
- History of Communications
- History of Computing
- ARPANET
- TCP/IP
- Packetization
- OSI Model
  
#### Hand on Lab
- Make an ethernet cable: https://www.wikihow.com/Create-an-Ethernet-Cable

## Lab 2 - Mikrotik Introduction
#### Lecture: https://docs.google.com/presentation/d/1nkGr8S5An02CQ5fo3RmMNeZxJ4dXIbm24C6_O8LXFJQ/edit?usp=sharing
- TCP vs UDP
- TCP 3-way handshake
- OSI Model
- Subnets
- DNS
- {Ports
- ICMP - Ping + Traceroute
- Firewalls
  
#### Hand on Lab

###### Set up Mikrotik : [Mikrotik-Lab.pdf](https://github.com/ereedsanchez/LABS-ISOC-Designing-and-Deploying-Computer-Networks/blob/4184522375c9b43be018cce71dd053a62cf25804/ISOC-DDCN-LAB2-Mikrotik-setup.pdf)
- If you are unable to download Winbox, you can also access MikrotikOS from 192.168.88.1
- Remember to connect your computr to the mikrotik in port 2, in the LAN section.ts 
- If you only have wifi, you can connect to your mikrotik, through the wifi SSID.  It will be the mikrotik and the last 6 digits of the MAC address of your wireless card. you can find this number on the sticker on the bottom of the Mikrotik router.

###### Let's make the internet
In the second part of this lab, we will emulate the making of the internet. Remember the internet is just a bunch of smallet networks connected. In the current configurations, your Mikrotik has no access to the internet or a WAN connection. You will connect your router to my router which does have internet, but you must properly configure your router or there will be conflicts!

1. Make 2 cables, one long cable to connect to my router that has internet, and one to connect the computer.
2. Login into the MikrotikOS, with Winbox, or 192.168.88.1
3. Go to Quickset.
4. Change your SSID names. make sure to have 2G and 5G at the end of your SSID names. Example: NextGenNet2G, NextGenNet5G.
5. Set an SSID password (optional)
6. Apply configurations.
7. Reconnect to your Mikrotik's SSID which you just changed.  (You got kicked off when you changed SSID names if you are connected via wifi)
8. Login again to MikrotikOs, and go to quickset.
9. Change the IP address to 192.168.xxx.1 - the xxx need to be changed to something that won't conflict with the Mikrotik you will connect to and give you internet. So it can't be 192.168.88.1.  Your professor will give you the correct ip to change to.
10. Change DHCP addresses to the same network as your IP address with a range from 10-254.  For example, if your IP is 192.168.90.1, your DHCP range will be 192.168.90.10-192.168.90.254.
11. Apply configurations.
12. Reconnect to MikrotikOS, if you are kickoff.  you will need to use the new IP address you just set to log in via the web browser. For example, if you change your IP address to 192.168.90.1, you will use that address to connect to the MikrotikOS.
13. Connect your WAN port to the Mikrotik that has internet.  If the main mikrotik router no longer has ports you can connect to your nieghbors Mikrotik router.
14. If you have internet, you can now claim you built a small portion of the internet by connecting your small lan network to a greater WAN network!  You are a winner!

[<img src="images/Mikro1.png">](https://github.com/ereedsanchez/LABS-ISOC-Designing-and-Deploying-Computer-Networks/blob/main/images/Mikro1.png)

