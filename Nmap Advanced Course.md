Certainly, here is a comprehensive list of various Nmap commands with explanations for each type:

1. Basic Scan:
Command: nmap target
Description: Perform a basic scan on the target host. This will scan the most common 1,000 TCP ports.
2. Scan All TCP Ports:
Command: nmap -p- target
Description: Scan all 65,535 TCP ports on the target host.
3. Scan Specific Ports:
Command: nmap -p port1,port2,... target
Description: Scan specific ports on the target host.
4. Service Version Detection:
Command: nmap -sV target
Description: Detect service versions running on open ports.
5. Operating System Detection:
Command: nmap -O target
Description: Attempt to identify the target's operating system.
6. Aggressive Scan:
Command: nmap -A target
Description: Enable OS detection, version detection, script scanning, and traceroute.
7. Fast Scan (Skip Host Discovery):
Command: nmap -F target
Description: Fast scan, targeting the most common ports. Skips host discovery.
8. Ping Scan:
Command: nmap -sn target
Description: Perform a ping scan to check if hosts are up.
9. UDP Scan:
Command: nmap -sU target
Description: Scan for open UDP ports.
10. Script Scan:
- **Command:** `nmap -sC target`
- **Description:** Scan using default NSE scripts.
11. Custom Script Scan:
- **Command:** `nmap --script scriptname target`
- **Description:** Run a specific NSE script against the target.
12. Scan Multiple Targets:
- **Command:** `nmap target1 target2 ...`
- **Description:** Scan multiple targets simultaneously.
13. Exclude Hosts from Scan:
- **Command:** `nmap target1 --exclude target2`
- **Description:** Exclude a specific host from the scan.
14. Save Output to a File:
- **Command:** `nmap -oN output.txt target`
- **Description:** Save scan results to a file in normal format.
15. Save Output in XML Format:
- **Command:** `nmap -oX output.xml target`
- **Description:** Save scan results to a file in XML format.
16. Verbose Output:
- **Command:** `nmap -v target`
- **Description:** Increase verbosity to get more detailed output.
17. Aggressive and Verbose Scan:
- **Command:** `nmap -A -v target`
- **Description:** Combine aggressive scan with increased verbosity.
18. IP Range Scan:
- **Command:** `nmap 192.168.1.1-254`
- **Description:** Scan a range of IP addresses.
19. Top Ports Scan:
- **Command:** `nmap --top-ports 10 target`
- **Description:** Scan the top 10 most common ports.
20. Fragmented Packet Scan:
- **Command:** `nmap -f target`
- **Description:** Send fragmented IP packets.
21. Idle Scan (Incremental Scan):
- **Command:** `nmap -sI zombie_IP target`
- **Description:** Perform an idle scan using a zombie host.
22. List Scan:
- **Command:** `nmap -sL target`
- **Description:** List IP addresses without scanning.
23. Firewall Evasion Techniques:
- **Command:** `nmap -f -g 53 target`
- **Description:** Use decoy and fragmentation techniques for firewall evasion.
24. TCP SYN Ping Scan:
- **Command:** `nmap -PS target`
- **Description:** Use TCP SYN packets for host discovery.
25. TCP ACK Ping Scan:
- **Command:** `nmap -PA target`
- **Description:** Use TCP ACK packets for host discovery.


These are just some of the commonly used Nmap commands. The tool is highly versatile, and you can customize scans based on your specific needs and the nature of the target network. Always ensure that you have the necessary permissions before scanning any network or system, as unauthorized scanning may be against the law and could result in legal consequences.