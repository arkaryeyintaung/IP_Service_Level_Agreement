### When interface is suddenly down!
![image](https://github.com/user-attachments/assets/ba3a3c99-e5f9-407f-ad5c-626d323866e1)

---

### This log message indicates that the IP SLA tracking object (1) associated with SLA operation 1 has changed its state from Up (reachable) to Down (unreachable). The ICMP echo request (ping) to the monitored IP (10.0.1.2) failed.
![image](https://github.com/user-attachments/assets/9a1bd5d0-e221-4b89-88c9-03b770907dc8)

---

### Now, the primary link becomes unreachable, the tracking object goes Down, and the primary route is removed from the routing table. When the primary route is removed, the router automatically uses the secondary route (with higher AD) as the active route.
![image](https://github.com/user-attachments/assets/f4e29556-9481-4cc7-81b0-debd5622b91b)

---
### When the primary link becomes operational again (IP SLA detects the next-hop is reachable), the tracking object changes to Up. The router automatically reinstalls the primary route in the routing table because it has a lower AD than the secondary route. Traffic shifts back to the primary link.
![image](https://github.com/user-attachments/assets/2d895844-d53c-4a88-8a38-35af0e5ddb1f)

---

## Conclusion

Thank you for exploring this repository! We hope you find the project helpful and informative.

## Support
If you like this project, consider giving it a ⭐ to show your support!

---
