# notes


Best practice before to configure routing , know 
1. ping = dikit (directly connected)
2. route not dikit 


!static routing recipe
ip route <not directly connected network IP> <subnet mask of NDCN> <Host IP of next hop>


!To clear static ip route command
conf t
 no ip routing
 ip routing
 end

======================================================================

!Dynamic Routing (EIGRP - OSPF - BGP)

EIGRP (Enhanced Interior Gateway Routing Protocol)
-best dynamic routing protocol
-administrative distance 90
-Cisco Proprietary (Only works on Cisco Devices)
EIGRP States: Hello > Query > Update > Received > Acknowledge


command:
show ip protocols = to know Autonomous System Number (AS Number)


=====================================================================

OSPF Routing (Open Short Path First )
- Multi Vendor Dynamic Routing Protocol
- Link State Advertisement
- Implements Dijkstra Algorith
- Advertised by AREA (Area 0 is the Backbone)
OSPF StatesL Down > Init(Initialized) > Two-way EXSTART > EXCHANGE > LOADING > FULL 


==============================================================
BGP Routing (Border Gateway Protocol)
- Mostly used for Wide Area Network (WAN)
- Also used by ISPs and Large Corporations 

BGP Messages
(NOKU Packets: Notification, Open, Keep-Alive, Update)
clear ip bgp * soft !updates BGP Advertisements upon modification of BGP Attributes

Route Redistribution
(by default, different routing protocols cannot get along each other)



**************************************************************************************************
DAY 4
Task 1:  Fundamentals of Network/

Physical layer = Bits

V - Voltage
I - Interface
T - Transmission



OSI Layer
Application 7 - Data "Bytes"
Presentation 6 - Data Format (File Format) (Ex. jpeg, gif, img)
Session 5 - Data Stream
Transport 4 - Segment (source port and destination port)
Network 3 - Packets (source ip and destionation ip)
Data Link 2 - Frames 
Physical 1 - Bits
3 Ways for transmission
1. Fiber Optic
2. Radiofrequency
3. Electrical 


Task 2:
Layer 3 Attack: nmap -sP 10.k.1.0/24

Layer 4 Attack: -v 10.k.1.0
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds

Layer 5 Attack: 
net use x: /delete
net use \\10.k.1.10\ipc$


Layer 7: nakawin ang drive C: ni kalaban, gawing drive mo

net use x: \\10.k.1.10\c$

How to know if na hack ka
netstat -s -p tcp








































































