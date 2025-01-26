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















