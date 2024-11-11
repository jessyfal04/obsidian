---
draft: true
---
# Process
## Beginning
I decided to : 
- Try using the UDP Hole Punching methods.
- I use my VPN as a STUN server.
- Coding in C++
## Under the same NAT limitation
- When B and C share the same public IP the chat can't occur.
- 


# Failures / Difficulties
## UPnP Approach

`sudo apt-get install miniupnpc`
`g++ upnp.cpp -o upnp -lminiupnpc`

![[Pasted image 20241010114640.png]]
Not working, the program says that no UPnP's device is available.