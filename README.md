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


!Dynamic Routing (EIGRP - OSPF - BGP)

EIGRP (Enhanced Interior Gateway Routing Protocol)
-best dynamic routing protocol
-administrative distance
-Cisco Proprietary (Only works on Cisco Devices)









