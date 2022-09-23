###### Back to [[CMPUT 404]]
---
# Link Layer
___
## Important Links
- 
___
## Definitions

- 

___
## Notes
### Ethernet Frame
- A frame is a data packet/unit thats around 64 to 1568 bytes.
- Preamble; 7 bytes, used to show the highest frequency signal sendable. Normally 0b10101010 or 0xAAAAAAAAAAAAAA
- SFD; (Start Frame Delimiter) 1 byte, indicates the start of a a frame. Normally 0xAB
- Destination MAC; 6 bytes, a MAC address of the reciever.
- Source MAC; 6 bytes, a MAC address of the sender.
- Length; 2 bytes, indicates the size of the payload.
- Payload; 46 - 1500 bytes, contains the data. Follows MTU (maxiumum transfer unit of 1500). If data is not 46 bytes, then pad with zeros.
- MTU ; Maximum transfer unit, used to standardize/maximum the amount of packet sizes. If the packet is too small, then too many headers will be sent. If packet is too large, then some recievers will not support a given size.
- CRC; Cyclic redundancy check, 4 bytes, used for error detection.
- MAC addresses are for local networks.

___
