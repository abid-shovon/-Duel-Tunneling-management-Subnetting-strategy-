# -Duel-Tunneling-management-Subnetting-strategy-
A Internet service provider(ISP) name Hexa link. They provide internet not only IPv4 but also IPv6 via DHCPv6 or Satically. 

Platform: Packet-Tracer

Networking Features: Dedicatedly used DHCPv6 server | Inter-Vlan (Layer-3 switch) | IPv4 & IPv6 |
Management IP for layer -2 switch |Routing (Static & OSPF) | L2 and L3 devices security |Port-Security
for Office network only | Telnet & SSH | TFTP server for backup.


Some information of this lab: 

Ip block information:
main Block: 192.168.10.0/23

Marketing 200 users 192.168.10.0/24
Gateway: 192.168.10.1
Vlan 2

IT 120 users 192.168.11.0/25
Gateway: 192.168.11.1
Vlan 3

CEO 2 users 192.168.11.160/30
Gateway: 192.168.11.161
Vlan 4

technical 10 users192.168.11.128/28
Gateway: 192.168.11.129
Vlan 5

Management IP of Hex-link:

L2 switch-1: 192.168.11.172/30
Default gateway 192.168.11.173

L2 switch-2: 192.168.11.176/30
Default gateway 192.168.11.177

L2 switch-3:
192.168.11.180/30
Default gateway 192.168.11.181

For TFTP server:
10.10.10.0/30

-------------------------------------------------------------------------------
L2 & L3 SW same conf.

vtp mode Client 
vtp domain shovon
vtp password shovon4333
--------------------------------------------------------------------------------
L3 Distribution SW

vtp mode Server 
vtp domain shovon
vtp password shovon4333
---------------------------------------------------------------------------------
All router and switch have common password:
password: hexalink
---------------------------------------------------------------------------------

