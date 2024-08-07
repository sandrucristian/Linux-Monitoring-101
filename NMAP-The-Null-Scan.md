# The Null Scan 
- **You’re being watched**

```
nmap -sN 192.168.1.10
```
  
The Null Scan is a type of TCP scan that hackers — both ethical and malicious — use to identify listening TCP ports. In the right hands, 
a Null Scan can help identify potential holes for server hardening, but in the wrong hands, it is a reconnaissance tool. It is a pre-attack probe.

`A Null Scan is a series of TCP packets that contain a sequence number of 0 and no set flags.`

In a production environment, 
there will never be a TCP packet that doesn’t contain a flag. Because the Null Scan does not contain any set flags, 
it can sometimes penetrate firewalls and edge routers that filter incoming packets with particular flags.

The expected result of a Null Scan on an open port is no response. Since there are no flags set, the target will not know how to handle the request. 
It will discard the packet and no reply will be sent. If the port is closed, the target will send an RST packet in response.

Information about which ports are open can be useful to hackers, as it will identify active devices and their TCP-based application-layer protocol.

Cisco NetFlow packets contain a summary of the packets flowing through an interface including TCP flags, or in this case, not set. 
Cisco NetFlow coupled with a behavior analysis tool can help identify when Null Scans are occurring on your network.

Reference

https://www.plixer.com/blog/the-null-scan-youre-being-watched/#:~:text=A%20Null%20Scan%20is%20a,doesn't%20contain%20a%20flag.

![AdminsWatchingGIF](https://github.com/user-attachments/assets/5eed39fc-82fa-4310-9920-b819fb87c78e)
