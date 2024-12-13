```
ip sla 1
icmp-echo 10.0.1.2
timeout 5000
frequency 10
exit
ip sla schedule 1 start-time now life forever
no ip route 0.0.0.0 0.0.0.0 10.0.1.2
ip route 0.0.0.0 0.0.0.0 10.0.1.2 track 1
track 1 ip sla 1
```
