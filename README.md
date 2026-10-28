# NETWORKWALKS-GLORIA-B084D-WK1-PM1-CYBERSECURITY-LAB-SETUP
For cybersecurity
# Cybersecurity Lab Setup - Week 1

## Task Completed
1. VirtualBox Latest Installed
2. Kali as attacker machine
3. Network 10.0.0.0/24 NATNetwork
4. Clipboard & Drag&Drop Enabled
5. Shared Folder = Downloads
6. Kali IP = 10.0.0.2/24
7. Internet Working

## Screenshots

### 1. VirtualBox Network Manager 10.0.0.0/24
[Upload screenshot here] <img width="1366" height="768" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/1fda348a-8bae-4092-8d80-2a29c3bbc289" />



### 2. Kali VM Network Setting - NAT Network
[Upload screenshot here] <img width="1366" height="768" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/47d6c295-66a7-476e-8c65-8967930f1d9a" />


### 3. Clipboard Bidirectional
[Upload screenshot here <img width="1366" height="768" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/42725460-ee85-42cd-90de-dfd8828014e0" />


### 4. Shared Folder Downloads
[Upload screenshot here] <img width="1366" height="768" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/ed97d123-5fe2-4c08-82ed-1ea96fb67e08" />


### 5. Kali IP 10.0.0.2 + Ping 8.8.8.8
[Upload screenshot here] <img width="1366" height="643" alt="image" src="https://github.com/user-attachments/assets/aaa77ba4-0a92-43cb-a146-134068b79ab9" />


## Troubleshooting
Issue: My IP kept going back to 10.0.0.3 and internet went off with "Network unreachable" after ip flush.
Solution: 
- Ran sudo ip addr flush dev eth0
- Ran sudo ip addr add 10.0.0.2/24 dev eth0

---
Acknowledgement
Thanks to `@waqaskamranccie` for the lab guide

Solution: Deleted Wired connection 1 and recreated with nmcli con add type ethernet ifname eth0 ipv4.method auto
