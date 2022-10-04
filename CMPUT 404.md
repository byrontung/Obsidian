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
- Largest UDP message you can send with fragmentation is 65508 bytes
- End headers with "\\r\\n"
- All URLs are URIs but not all URIs are URLs.
	- URI is more of a name, vs URL is more of the address of the name.
	- URI -> universal resource identifier
	- URIs have two subclasses -> URNs and URLs
- URL Format
	- Scheme : authority -> user:password (optional) hostname :post (optional) -> path -> ?query (optional) -> \#argument (optional)
	- Comes in the scheme and then everything else.
	- http, https, mailto, file, data
- HTTP Commands are made into a URI.
	- GET - Retrieve information from the URI.
	- POST - Run search, log-in, append data, change data.
	- HEAD - GET without a message body (for caching).
	- PUT - Store the entity at the URI.
	- DELETE - Delete the resource at that URI.
- ![[Pasted image 20221004034940.png]]
- They also have absolute and relative options as well
	- http://[::1]:8000/images/web-server.svg
		- Absolute authority, absolute path
	- http://[::1]:8000/images/../index.html
		- Absolute authority, relative path
	- /images/web-server.svg
		- Implied authority, absolute path
	- images/web-server.svg
		- Implied authority, relative path
- We are allowed to use Python URI Unicode UTF-8 encoders
	- Only use encoders when the character is not  ` -._0-9a-zA-Z`
	- Unless its the domain name, then we use punycode
### Queries
- Can have more than one or more arguments with an ampersand/semicolon to connect multiple queries.
- In the form  `key=value&key2=value2 `
### Fragments
- Where the # starts.
- Fragment is not sent to the webserver.
- The purpose is to jump to a certain point of the link.
	- Time from youtube, id of an element in the DOM.
- 
___
