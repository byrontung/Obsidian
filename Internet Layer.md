###### Back to [[CMPUT 404]]
---
# Internet Layer
___
## Important Links
- 
___
## Definitions

- Protocol is an agreement on how to communicate.

___
## Notes

- IPV4 ; A routing standard that allows Ethernet frames/data to be routed because we are provided addresses. Designed to be stateless. Limited IPV4 addresses. 
	- 32 bits for address space.
![[Pasted image 20220923114325.png]]  
- IPV6 ; Like IPV4 but with more addresses. Ex: (2001:0bd8:0000:0000:0000:0000:0000:00001, 3132:0:0:0:0:0:0:1, 2001:bd8::1)
	- 128 bits of address space.
	- IPV6 normally does not normally get fragmented
![[Pasted image 20220926123548.png]]
- Addresses here are global networks.
- UDP - User Datagram Protocol.
	- Provides checksums, and port numbers.
	- Stateless, lossy, and unordered.
	- No connections, and no guarantees but really fast.
![[Pasted image 20220926130502.png]]
- One UDP header is needed per message.
	- If the message is long, then there is still only one message.
	- IP handles fragmentation for us, it is needed to know when fragmentation is done.
## DNS - Domain Name Service
- Allows names to be binded to an IP or a set of IPs.
- Works on both IPV6 and IPv4.
- host, dig, nslookup can be used to check names.
- Records:
	- A - Points to an IP
	- CNAME - records point to another name.
	- MX - for mail
___