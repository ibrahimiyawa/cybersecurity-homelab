# cybersecurity-homelab
Built a virtual lab environment for practicing cybersecurity skills in an isolated, safe network.
# Cybersecurity Homelab Setup

## Components
- **Virtualization Platform:** Oracle VirtualBox
- **Attacker Machine:** Kali Linux 2024.1
- **Target Machine:** Metasploitable 2
- **Network Configuration:** Internal network ("cyberlab")

## Setup Steps
1. Downloaded and imported Kali Linux OVA
2. Created Metasploitable2 VM from VMDK
3. Configured both VMs on internal network `cyberlab`
4. Verified connectivity with ping and initial nmap scan

## Initial Security Assessment
Performed basic reconnaissance on Metasploitable2:
- Discovered 20+ open services using `nmap -sV`
- Successfully exploited vsftpd 2.3.4 backdoor vulnerability
- Gained root access via Metasploit Framework

## Network Diagram
[Host Machine]
|
[VirtualBox]
├── Kali Linux (192.168.56.102) - Attacker
└── Metasploitable2 (192.168.56.101) - Target

## Skills Demonstrated
- Virtual machine configuration and networking
- Basic Linux command line proficiency
- Network reconnaissance with Nmap
- Vulnerability exploitation with Metasploit
- Safe, isolated lab environment creation
