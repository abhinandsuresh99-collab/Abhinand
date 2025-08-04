Objective

The goal of this task is to scan my local networkusing nmap identify open ports and services and understand the potential security risksfrom exposed services. 

---

Tools Used
 Nmap- For scanning network IPs and detecting open ports/services
 Windows Command Prompt For network info ipconfig
 
Steps Performed
1. Identified Local IP and Subnet
Found my device’s IP address:
Ran Nmap TCP SYN Scan on Local Network:nmap -sS 192.168.1.0/24
 Detected Open Ports and Services
Nmap scan report for 192.168.1.5
PORT     STATE SERVICE
22/tcp   open  ssh
80/tcp   open  http
443/tcp  open  https

Nmap scan report for 192.168.1.10
PORT     STATE SERVICE
135/tcp  open  msrpc
445/tcp  open  microsoft-ds
Researched Common Services on Open Ports
22	SSH	Remote shell login (Linux)	Medium
80	HTTP	Web server, unencrypted	Medium
135	Microsoft RPC	Windows Remote Procedure Call	High
445	SMB	File sharing on Windows	High
