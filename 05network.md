# Private ip address 
is provided by the router to coummunicate with the other devices connected to that network or router

# Public ip address 
is provided by ISP which represent the all the devices connected to the router, it is basically the ip adress provided to the router by ISP.

IP address is not permanent it is only provided by network, if you are not connected to router then device may have ip address but that is not active

# Mac address
MAC address:
    A unique identifier burned into the hardware of your computer's network interface card (NIC).
    Assigned by the manufacturer and practically permanent. In rare cases, some manufacturers might allow specific tools to change it.
    Used on the local network level (like a LAN) for identifying devices and allowing communication


IP address:
    Assigned by a network (like your router or ISP) to identify your device for communication.
    Can be public (facing the internet) or private (within your local network).
    Not permanent and can change depending on the network configuration.


# Network Address Translation (NAT) is a technique used
 in networking to remap one IP address space into another by modifying network address information in the IP header of packets while they are in transit across a traffic routing device. NAT allows multiple devices within a local network to share a single public IP address for internet access.


Basic NAT: For example, if a device with a private IP address of 192.168.1.2 wants to access a website on the internet, the router translates the source IP address to its own public IP address before forwarding the packets to the internet.





# ifconfig 
on windows # ipconfig 
all details about network configuration

# ping www.google.com
for check net connectivity from your server to google.com


# curl ifconfig.me
   This is the address visible to the internet and isn't permanent.
# curl -4 icanhazip.com  # For IPv4 specifically
  OR (For IPv6)
# curl -6 icanhazip.com
<!-- How to check if  a IP:PORT is accessible and open or not -->
# telnet IP Port 


# ifconfig | grep ether 
This command displays information about your network interfaces. The grep ether part filters the output to only show lines containing "ether," which indicates the MAC address. 



<!-- How to check al hubs in network path to reach a website -->
# traceroute
# reboot
# shutdown


# sudo apt-get install tcpdump

# sudo tcpdump -v
tcpdump: listening on eth0, link-type EN10MB (Ethernet), capture size 262144 bytes

# sudo tcpdump -vv
tcpdump: listening on eth0, link-type EN10MB (Ethernet), capture size 262144 bytes

we recieve the packets form where packets are coming

# sudo tcpdump -c 10 -vv

<!-- How to check if port is open or not on our server and to identify no. of connection on a given port or IP -->
# netstat -putan | grep 80
 // putan : proces udp tcp all numeric

  netstat command is a cmd line network utility that displays: 
  Network connections for TCP, UDP 
  Routing tables
  a number of network interface network protocol


# netstat -an | grep 12345 


# netstat | more
# netstar -l 
    -l used for listening state

# netstat -r
    for routing table;

# netstat -i 
     interface














