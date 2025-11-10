# A Cheat Sheet For Ports.

A useful reference for ports with their names and functions/services that they support.

 Not every port is listed here as I wanted to focus on common ports seen in security related scenarios. I may also update the table with known risks with these ports and why they should be monitored for unusual behavior.

 There are 3 main categories of ports.
    
## Well known ports.
Ports 0 - 1023.

These ports are assigned system ports that. They are used by system processes that use types of network services.


|Port|Description|
|---|---|
|20 | FTP - File Transfer Protocol (data transfer). A standard communication protocol used for the transfer <br> of computer files from server to client.|
|21 | FTP - File Transfer Protocol (command). This port is used as the control channel for sending commands and receiving responses between FTP client and server.|
|22 | SSH - Secure Shell. A cryptographic network protocol for operating network services securely. Notable applications are remove login and command line execution.|
| 23 | Telnet - Unencrypted text communications. Should not be used for applications such as remote management as all information is transferred in plain text.|
| 25 | SMTP - Simple Mail Transfer Protocol. Internet standard communication protocol for email transmission. Mail servers use SMTP to send and receive mail messages.|
| 42 | Host Name Server Protocol - An obsolete network protocol used in translating a host name to an Internet address. Now more commonly used by WINS though this is also considered obsolete and should not be used on networks not requiring it.|
| 43 | WHOIS - A query and response protocol that is used for querying databases that store an internet resource's registered users or assignees. | 
|53 | DNS - Domain Name Service. A service that provides a naming system for computers, services and other resources on the Internet or other IP networks.|
| 69 | TFTP - Trivial File Transfer Protocol. A simple lockstep communication protocol for transmitting or receiving files in a client-server application. Primary use in early stages of nodes booting on a LAN when OS or firmware ISOs are stored on a file server.|
| 80 | HTTP - Hypertext Transfer Protocol. The foundation of data communication for the WWW.|
| 88 | Kerberos - A computer-network auth. protocol that uses tickets to allow nodes communicating over unsecure networks to proves their identity to each other in a secure manner.|
| 110 | POP3 - Post Office Protocol V3 - Used by email clients to retrieve emails from a mail server.|
| 119 | NNTP - Network News Transfer Protocol.  an application protocol used for transporting Usenet news articles between news servers, and for reading/posting articles by the end user client applications.|
| 143 | IMAP - Internet Message Access Protocol. A standard internet protocol used by email clients to retrieve email from a mail server.|
| 443 | HTTPS - An extension of HTTP. It uses encryption for secure communication over a computer network and widely used over the Internet.|
| 465 | SMTPS - SMTP over TLS protocol, a cryptographic protocol that protects Internet communications.  |
| 563 | NNTPS - NNTP over TLS/SSL protocol.| 
| 993 | IMAPS - IMAP over TLS/SSL protocol.| 
| 995 | POP3S - POP3 over TLS/SSL protocol.|
| 989 | FTPS - FTP over TLS/SSL protocol, data transfer. |
| 990 | FTPS - FTP over TLS/SSL protocol, control. |

## Registered ports.
Ports 1024 - 49151.

These ports are a dynamic port number that are assigned by IANA (Internet Assigned Numbers Authority) for specific services upon application by a requesting entity. 

While these ports are assigned and registered to an entities application on most systems these ports can be used without superuser/admin privileges.

These applications have a wide range of functions from security tools to video game chat or communication services.

|Port | Description | 
|---|---|
|1080| SOCKS - An Internet protocol that exchanges packets between a client and server through a proxy server.|
|1119 | Battnle.net - Battle.net's chat/game protocol used by Blizzrd's games.|
|1194 | OpenVPN - Used by OpenVPN's VPN service.|
|1242 | Nessus Security Scanner - a vulnerability scanner developed by Tenable Inc.|

These are just a few examples.

## Dynamic, Private or Ephemeral ports.
Ports 49152 - 65535.

These are private or dynamic ports that cannot be registered with IANA. These are used for private or customized services.
Some of these ports are commonly used by well known entities and considered standardized though not official. 
