# DNS-Tunneling-Presentation
Gaining a Command Shell by Tunneling Through DNS, Presentation done while studying for degree.

This powerpoint is a project I did for my degree. I created a small LAN in GNS3 hosting 2 VM's, an attacker and a target, separated by a router running a restrictive ACL only allowing for DNS traffic and HTTP traffic.

The goal is to obtain a command and control connection via exploitation of the vulnerable HTTP service. (picked out ahead of time using exploit DB with simplicity in mind as the buffer overflow is not the point here.)

The primary tools used were DNScat2-powershell, and Metasploit/MSFVenom, to construct a custom payload that instead of invoking some stock shellcode, will launch CMD and run a Base64 encoded powershell command to download and run the dnscat2 script.

All tools and resources used are cited in the powerpoint's PDF itself. 

Unfortunately I lost the files used for this project and may recreate it at some point if people are interested. 
