###### Back to [[CMPUT 404]]
---
# Internet Layer
___
## Important Links
- 
___
## Questions
- 
___
## Definitions

- Protocol is an agreement on how to communicate.

___
## Notes

- IPV4 ; A routing standard that allows Ethernet frames/data to be routed because we are provided addresses. Designed to be stateless. Limited IPV4 addresses. 
	- 32 bits for address space.
	- 20 byte minimum header.
![[Pasted image 20220923114325.png]]  
- IPV6 ; Like IPV4 but with more addresses. Ex: (2001:0bd8:0000:0000:0000:0000:0000:00001, 3132:0:0:0:0:0:0:1, 2001:bd8::1)
	- 128 bits of address space.
	- IPV6 normally does not normally get fragmented
![[Pasted image 20220926123548.png]]
- Addresses here are global networks.
## Special IPs and Ports
- 127.0.0.1 localhost (packets that loop back to your computer)
- 192.168. * . * and 10. * . * . * are for common private subnets for IP communication
- TCP Port 80 - HTTP
- TCP Port 443 - HTTPS
- UDP Port 53 - DNS
## UDP - User Datagram Protocol.
- Provides checksums, and port numbers.
- Stateless, lossy, and unordered.
- No connections, and no guarantees but really fast.
![[Pasted image 20220926130502.png]]
- One UDP header is needed per message.
	- If the message is long, then there is still only one message.
	- IP handles fragmentation for us, it is needed to know when fragmentation is done.
## TCP - Transmission Control Protocol
- ![[Pasted image 20221001154103.png]]
- 20 byte header.
- Also sits on top of IP.
- Connection/stream oriented
	- Data can come bidirectionally
- 3-packet handshake
	- I send hello, they acknowledge the hello, I achnowledge their achnowledgement
	- ![[Pasted image 20221001154534.png]]
- Acknowledge revieving of handshake.
- Keeps order.
- Used by most internet applications.
- Used in HTTP, FTP, SMTP, IMAP, POP3, GOPHER, Telnet
## DNS - Domain Name Service
- Allows names to be binded to an IP or a set of IPs.
- Works on both IPV6 and IPv4.
- host, dig, nslookup can be used to check names.
- Records:
	- A - Points to an IPV4
	- AAAA - Points to an IPV6
	- CNAME - records point to another name.
	- MX - for mail
___