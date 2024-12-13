This configuration sets up NAT (Network Address Translation) to allow devices in the private network to share a single public IP for internet access

![image](https://github.com/user-attachments/assets/31dcd38b-024c-495b-854f-582cf69150b6)
```
For ISP-1 NAT-Config
---
access-list 10 permit any
ip nat inside source list 10 interface e0/2 overload
int e0/0
ip nat inside
exit
int e0/2
ip nat outside
```
```
For ISP-2 NAT-Config
---
access-list 10 permit any
ip nat inside source list 10 interface e0/1 overload
int e0/0
ip nat inside
exit
int e0/1
ip nat outside
```
