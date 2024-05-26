Network Concepts and Protocols


Network Concepts:

- What is networking?

What is data networking?

It’s more about transferring information. A system of hardware, software and protocols used to move information from one device to another.


- Communication Processes


Using the OSI Model to Describe Network Operations:

The OSI Model = Open Systems Interconnect

There are 7 in layers in the OSI Model:


1st – the Physical Layer – these are the cables we are using;
2nd – Data Link Layer – these are the protocols that will allow our computer and other devices to communicate locally with other devices;
3rd – Network Layer – that allows us to make use of the Data Link Layer and Physical Layer to send messages on distances across a network;
4th – Transport Layer – It uses TCP (Transmission Control Protocol)  – it sets up a session between our work station and the server, so that we can send data between these two devices;
5th Session Layer;
6th – Presentation Layer; 
7th – Application Layer;

Encapsulation and the OSI Model:

Users are being displayed the Application layer when they enter a website.
Any data we have with a header at the Transport layer is called a segment.
A chunk of data, with a network layer header is called a packet.

A chunk of data, with a Data Link layer is called a header.


Describe Protocol Uses and Port Numbers:

Application Layer Protocols:
- Data Transfer Protocols;
- Authentication Protocols;
- Network Service Protocols;
- Audio/Visual Protocols;
- Database Protocols;

Transferring files:
HTTP has port 80.
HTTPs has port 443.

So port 80 and 443 we typically associate with using web services. When you are using HTTPs on port 443 you will often hear talk about SSL (Secure Socket Layer) or TLS (Transport Layer Security). They are the same thing. It is the same protocol, they just changed it’s name. We use it to provided encryption when we are using HTTPs.

These are all transfer file protocol of some kind:
FTP = File Transfer Protocol. It operates on two ports – 20/21. 
sFTP =  secure File Transfer Protocol. It operates on port 22, it is FTP with encryption.
TFTP = Trivial File Transfer Protocol.  It operates on port 69. It’s going to be used to transfer small files
SMB = Server Message Block. It operates on port 445.

There are 3 methods we are going to need to transfer an email:
- POP3
- IMAP
- SMTP

Authentication and DHCP:

There are two protocols we are going to use for this and they are:
- LDAP – Lightweight Directory Access Protocol. It uses port number 389.
- LDAPs – Lightweight Directory Access Protocol secure. It uses port number 636.

Note: When a protocol ends with ‘s’, this means it is encrypted. When there is no ‘s’, it means it isn’t encrypted. 

Network Services:
- DHCP = Dynamic Host Configuration Protocol; It uses ports 67/68 in order to operate on a network.

Command:

ipconfig /release – release ip, so the user doesn’t have one;
ipconfig /renew – gives the user a new ip address;


- DNS = Domain Name Service/System

It allows us to take names for `google.com`, `facebook.com`, etc. and it allows us to take the name into an ip address, so that we can use the ip address to transfer information at the network layer. In other words it resolves names. It works on port 53. The port for encrypted is 443.

Command:

nslookup – this command will ask to resolve a host name. It will tell me the ip address and then it gives me a list of ip addresses for pluralsight.
example: nslookup pluralsight.com
example 2: nslookup google.com


- NTP = Network Time Protocol
It’s a device on the network that has a clock on it. It has a very precise time. If an event is happening we are going to know the precise time it is happening.

Network Management Protocols:
- Telnet
- Secure Shell
- SNMP = Simple Network Management Protocol.  It uses ports 161/162.
- Syslog = operates port number 514.
- RDP = Remote Desktop Protocol. It allows us to enter remote user desktops on our network when we are on local. This operates on port number 3389.
- SIP = Session Initiation Protocol. It operates on port numbers 5060/5061.


SQL Database Protocols:
- mySQL = operates on port number 3306;
- SQLnet  = operates on port number 1521;
- SQL Server  = operates on port number 1433;

TCP and UDP:

- Transmission Control Protocol (TCP) – a protocol that initiates communication between two devices.
The 3-way Handshake:
SYN message – it’s the first message to the web server indicating that the client wants to start a conversation
SYN-ACK – it’s just alerting the client that the user is available for the conversation.
ACK – acknowledgment.

The 4-way Disconnect: a FIN, respond with a FIN-ACK. The client is going to reply with it’s own FIN message and server is going to reply back to that with a FIN-ACK.

TCP Reset – it can come from both the client and the server.


- User Datagram Protocol (UDP) – works similarly to TCP, but this time we directly start to communicate. There are no 3-way handshakes, no 4-way disconnect. There are no reset’s. No reliable communication, no sequence numbers, no acknowledge numbers. It’s used for efficient data transfer.

Protocol Hierarchy 

Transport layer is responsible for building a session and maintaining a session between two endpoints, typically a client and a server.

Port Numbers:
- Server Port Numbers – Well known numbers / registered /. They go from 0 to 1023.
- Client Port Numbers – ephemeral Port Numbers. They go from 1024 to 49 151. They are used by the client to identify the session.

Introduction to Binary and Hexadecimal:

In order to get the hexadecimal, we must get the binary number first and after that we find what’s the hexadecimal.

Example for a number: 1001 (2)

Introducing IPv4 Addressing:

The network layer is where we use IP addressing to get messages from one device to another device on the internet.


Example of an IP address: 203.0.113.10

Network Portion: 203.0.113
Host Portion: 10

IP Address Construction:

An IP address is consisted of 4 octets. An octet is just a set of 8 bits and there are 4 sets of 8 bits.

203.0.113.10 = 11001011 00000000 01110001 00001010

Classful Addressing (-1995 and prior)
There are 5 different classful address:
Class A: from 0.0.0.0 to 127.255.255.255
Class B: from 128.0.0.0 to 191.255.255.255
Class C: from 192.0.0.0 to 223.255.255.255
Class D: from 224.0.0.0 to 239.255.255.255
Class E: from 240.0.0.0 to 255.255.255.255

The first three classes are called unicast addresses and these are the addresses we use on the internet. Class D addresses are for multicast. Class E is for experiments. In classful addressing, the class of the address determines the division between the network and the host portion.



Classless Addressing (-1995 to present)

Subnet mask: it’s consisted of a series of ‘1`s’, followed by a series of 0`s.

Example: 203.0.113.10
Subnet Mask: 11111111 11111111 11111111 00000000
255.255.255.0

Example 2: 10.0.0.10
00001010 0000000 00000000 00001010
11111111.0000000.0000000.0000000
255.0.0.0