# Elevate-Lab-Internship
 Tasks Related to Internship


Day 1\
Date : 23/06/2025\
Difficulty : Easy


## Task 1
### Install Nmap using APT

```sudo apt update && sudo apt install nmap -y```

## Task 2
### Finding Local IP Range\
Tool : ip

Finding Ip & Subnet\
```ip addr show```

\
Please Check **images/ip_command_output.png** for more details


Finding Devices in Local Network\
```sudo nmap -sP 10.0.2.0/24```

\
Please Check **images/nmap_ping_scan.png** for more details


## Task 3
### Running Nmap TCP Syn Scan

```sudo nmap -sS 10.0.2.0/24```

\
Please Check **images/nmap_syn_scan.png** for more details


## Task 4
### Ports Open

Port 21 : FTP (File Transfer Protocol)\
Port 22 : SSH (Secure Shell)\
Port 23 : Telnet\
Port 25 : SMTP (Simple Mail Transfer Protocol)\
Port 53 : DNS (Domain Name Server)\
Port 80 : HTTP\
Port 111 : rcpbind\
Port 139 : netbios-ssn\
Port 445 : microsoft-ds\
Port 512 : Remote Execution Protocol(exec)\
Port 513 : login (rlogin)\
Port 514 : Shell (service)\
Port 1099 : rmiregistery\
Port 1524 : ingreslock\
Port 2049 : nfs\
Port 2121 : ccproxy-ftp\
Port 3306 : mysql\
Port 5432 : postresql\
Port 5900 : vnc\
Port 6000 : x11 (session)\
Port 6607 : irc\
Port 8009 : ajp13\
Port 8180 : Unknown (But Open)\


# Task 5
## Capturing Packets on Wireshark

For Capturing Packets on wireshark do the below steps\
* Start Wireshark\
* Select NIC to capture\
* After Capturing you can analyze the packets or save it to a file

\
Read **Media/Wireshark Packets Files/wireshark_output.pcapng** directory for more details


# Task 6
## Information About common services on Ports


FTP (port 21): Used for transferring files.\
SSH (port 22): Used for secure remote login and command execution.\
DNS (port 53): Used for resolving domain names to IP addresses.\
SMTP (port 25): Used for sending emails.\
HTTP (port 80): Used for unencrypted web traffic.\
HTTPS (port 443): Used for secure web traffic (encrypted with SSL/TLS).\
POP3 (port 110): Used for retrieving emails.\
IMAP (port 143): Used for managing emails on the server.\
NetBIOS (ports 137, 138, 139): Used for file and printer sharing on Windows networks.\
RDP (port 3389): Used for remote desktop access to Windows systems.\
MySQL (port 3306): Used for the MySQL database system.\
PostgreSQL (port 5432): Used for the PostgreSQL database system.\
VNC (port 5900): Used for remote desktop sharing.


# Task 7
## Potential Security Risks from open ports

* Outdated Services -> These Open Ports could be running services which are outdated which might be vulnerable to attacks
* Information Disclosure -> These Open Ports could disclose information which the admin doesn't want outsiders to know like which services does the system runs
* Statistical Attack -> An attacker could run attacks which are persistent which will eventually let attacker gain access to the system
* Malware Infections -> An attacker could use open ports to inject malware into the system thus crashing the entire system



# Task 8
## Saving Nmap Scan Results to the file

```sudo nmap -sS 192.168.84.0/24 -oN output```

\
For More Details check **Media/Nmap Results/output**







