Villain Framework Reverse Shell Report
⚙️ Setup Info
Payload: windows/reverse_tcp/powershell

LHOST: 192.168.1.8

LPORT: 4444

🔁 Payload Delivery Method
The payload was executed on the target Windows 10 virtual machine using a PowerShell one-liner. This was done in a controlled lab environment, with the attacker machine running Kali Linux (hosting the Villain framework) and the target machine running on VMware. The payload was manually executed in the Windows PowerShell terminal to establish the reverse connection.

🖥️ Captured Info
Hostname: DESKTOP-UACST4S

IP Address: 192.168.1.9

User: desktop-uacst4s\lab
🔎 Enumeration Performed
powershell
Copy
Edit
whoami
# Output:
desktop-uacst4s\lab

ipconfig
# Output:
Windows IP Configuration
Ethernet adapter Ethernet0:
   Connection-specific DNS Suffix  . : 
   IPv4 Address. . . . . . . . . . . : 192.168.1.9
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : 192.168.1.1

systeminfo
# Output:
Host Name:                 DESKTOP-UACST4S
OS Name:                   Microsoft Windows 10 Pro
OS Version:                10.0.19045 N/A Build 19045
System Manufacturer:       VMware, Inc.
System Model:              VMware Virtual Platform
System Type:               x64-based PC
Processor(s):              1 Processor(s) Installed.
                           [01]: Intel64 Family 6 Model 142 Stepping 10 GenuineIntel ~2592 Mhz
BIOS Version:              VMware, Inc. 6.28, 05-07-2023
Total Physical Memory:     2,048 MB
