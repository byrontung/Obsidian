###### Back to [[Fall 2022]]
---
# CMPUT 404 - Web Applications and Architecture
## Important Links
- [TCP Packet Naming](https://www.howtouselinux.com/post/tcp-flags) 
## Questions
- What is the difference between address and destination in the ethernet vs IP
## Definitions
- Web ; Network of software/virtual pages (Wiki pages, blog posts, etc.) which is connected by hyperlinks, redirects, images, videos, HTML, etc.;
- Internet ; Network of computers/hardware (desktops, laptops, phones, etc.) which is linked by wifi, ethernet, cell towers, satelites, etc;
- HTML ; HyperText Markup Language. Information sent from web servers to web browers.;
- HTTP ; HyperText Transport Protocol. The connection used to connect web servers to web browsers.;
- Link Layer ; Lowest layer in the Internet protocol suite.;
- Internet Layer ; 
- Port ; TCP/UDP connection address. Ex: TCP uses port 80 for communications.
- Flags Connections ; Flags are put on packets for computers to understand what to do with the sent message.
___
## Notes

- [[Link Layer]]
- [[Internet Layer]]
- Ethernet Vs. Web
	- Ethernet is for local connection while web is for global connections.
- TCP Flags:
	- SYN : Synchronize -> Packets that initiate connections.
	- ACK : Acknowledgement -> Packs that are used to confirm data packets have been receieved.
	- FIN : Finish -> Indicates that the connection is being torn down. Both sender and reciever should send FIN packets to ensure termination.
	- PSH : Push -> Indicate that data should be passed to application instead of buffered.
	- Private Vs. Public Networks
		- Private networks are IP addresses that are given from your router.
		- Public networks are IP addresses that are given from internet providers.
	- Layer ordering (largest to smallest): Physical, ethernet, IP, UDP, DNS
	- Largest UDP unfragmented message you can send is 1480 if you count UDP headers or 1472 including payload size of UDP message.
	- Largest UDP message you can send with fragmentation is 65508 bytes\
	- End headers with "\\r\\n"
	- 
___
