SimpleRouter
============

This project implements a fully functional IP router that routes real network traffic.

Goal of the Project
-------------------
The aim of the project is to implement the following basic router functionalities. The router is declared to be functioning correctly if and only if:
* The router can successfully route packets between the firewall and the application servers.
* The router correctly handles ARP requests and replies.
* The router correctly handles traceroutes through it (where it is not the end host) and to it (where it is the end host).
* The router responds correctly to ICMP echo requests.
* The router handles TCP/UDP packets sent to one of its interfaces. In this case the router should respond with an ICMP port unreachable.
* The router maintains an ARP cache whose entries are invalidated after a timeout period (timeouts should be on the order of 15 seconds).
* The router queues all packets waiting for outstanding ARP replies. If a host does not respond to 5 ARP requests, the queued packet is dropped and an ICMP host unreachable message is sent back to the source of the queued packet.
* The router does not needlessly drop packets (for example when waiting for an ARP reply).

Testing the Router
------------------
At a minimum, and in addition to the required functionality above, the router should successfully pass the following tests:
* Pinging both application servers in your topology.
* Pinging the interfaces on the router.
* Tracerouting  to both application servers.
* Tracerouting to the router interfaces.
* Downloading large files from the application servers.

For more information check Stanford <a href="http://yuba.stanford.edu/vns/assignments/simple-router/" target="_new">Virtual Network System</a>.

Partners
--------
* Wassim Itani
* Ahmad El Hajj

References
----------
Ayman Kayssi, American University of Beirut, <a href="http://staff.aub.edu.lb/~ayman/" target="_new">More</a>.
