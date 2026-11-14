# IT-Fundamentals

Home network diagram v1 https://drive.google.com/file/d/1tLmIzITN8gC97OJWGO8Jh4Y6nZf77eZp/view?usp=sharing



Core skills : Hardware \& Infrastructure, Core software \& OS, Operational Procedures.

Areas for improvement : Networking infrastructure, Security implementations, Administrative workflows



Week 1 Log entry:



W/C - 19th October



Hours studied: 8





What I learned:

Learned how to use GitHub repository to keep track of my progress for the duration of my learning.

Installed apps needed to support my learning such as VirtualBox for VMs, Anki for flashcards and packet tracer for simulating networks.

Took a packet tracer course on cisco networking academy that shows how to use the app.

Took some practice quiz questions to figure out my strong areas and weak areas.

Created a home network diagram version 1 based on my current knowledge.



Confidence 1-5:

5



Next weeks goal:

Learn the basics of networking and create flashcards. Use packet tracer to practice real time networking in a simulated environment.



\-------------------------------------------------------------



Packet Tracer Lab:



Connected 2 PCs through a switch and gave them a static ip address. Learned about subnet masks and network bits and host bits. IP address contains total of 32 bits.



Problem: PC0 could not ping PC1

Symptoms \& Evidence: Request timed out, cable lights green, ipconfig showed pc0 and pc1 ip addresses

Root cause: The PCs were on different networks (third octet was different as subnet mask was 255.255.255.0)

Fix: Changed the PCs ip address so the network was the same but the host bits were different.

Lesson: When cables are fine but devices cant talk, check their addresses and masks to see if they are on the same network.



SUBNET Masks can be made up of 8,16,24,25,26...32 network bits. This reduces the number of host bits so 32 means 0 usable host IPs.

A value of 255 (11111111 in binary) means that entire octet belongs to the network.

A value of 0 (00000000 in binary) means that octet belongs to the host (the individual device).

Intermediate values (such as 128, 192, 224, 240, 252, 254) combine network and host bits within that single octet.

255.255.255.0: The first three octets (255.255.255) lock down the network ID, while the last octet (0) is left for individual host devices.





Week 2 Log entry:



What I learned:

The OSI model, all 7 layers, Physical layer, Data link, Network, Transport, Session, Presentation and Application

The TCP/IP model which has 4 layers, is similar to the OSI model but compacts a few layers together. Network access layer which combines the physical and data link layer, network layer, transport layer and application layer which combines session, presentation and application.

Learned how to use packet tracer, connected 2 PCs through a switch and gave them IP addresses. Learned about ip addresses and subnet masks. How to convert ip to binary. Network and host bits that affect the ip address and subnet mask.

Learned what a packet and a frame are.



Confidence level: 4



Next weeks goal: Go more in depth about subnetting to understand how everything works together. Understand it further and implement it with packet tracer to gain experience using my knowledge in a practical way.



\------------------------------------------------------------



Week 3 Log entry:



Packet tracer labs:

Watched how a switch builds its MAC address table using ARP in packet tracer simulation mode by deleting both PCs ARP cache and pinging them. 



What I learned:

Subnetting, VLSM and FLSM.

Binary to decimal. Subnet masks and CIDR notations.

The subnetting method, how to find the network and broadcast address as well as usable range. I can now subnet a network an divide the network between multiple different departments with different numbers of devices.

Ethernet frames are used to communicate with devices in a local network using MAC addresses.

ARP is used by a switch by sending a broadcast signal to all IPs on a network asking which one has that specific MAC address.



Confidence level: 5



Next week goal: Learn routing basics, default gateways, static routes, VLANs, DHCP and NAT. Labs will include connecting two networks using two routers and a static route, then building a two-VLAN network routed by a single router.



\------------------------------------------------------------





















