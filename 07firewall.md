<!-- Firewall -->
A firewall is network security system that monitors and controls incoming and outgoing network tarffic based on rules defined. 

Basically used to determine and block untrusted network to access out system.

Firewall basically monitors the incoming and outgoing traffic.

# Types of firewall
    Software Based: Running on operating system 
    HardWare Based: A dedicated appliance with Firewall software between tow different network.
                   Organisations uses this kind of firewall to protect its whole network.

# Listing, Adding, Deleting firewalld rules!

# firewall-cmd --list-all
# firewall-cmd --get-services

# firewall-cmd --add-port=20201/tcp
# firewall-cmd --remove-port=20201/tcp

TO block incoming traffic from an ip
# firewall-cmd --add-rich-rule='rule family="ipv4" source address="192.168.0.0" reject'

To block outgoing traffic to a IP or URL

# firewall-cmd --direct --add-rule ipv4 filter OUTPUT 0 -d <IP> -j DROP

How to get ip of facebook.com 
# host -t a www.facebook.com
  www.facebook.com is an alias for star-mini.c10r.facebook.com.
  star-mini.c10r.facebook.com has address 157.240.23.35 


To block ICMP incoming traffic
# firewall-cmd --add-icmp-block-inversion




























