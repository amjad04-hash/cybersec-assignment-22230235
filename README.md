# cybersec-assignment-22230235
Student Name: Amjad Ahmad
Student ID: 22230235
Malware Name: malware.exe
SHA-256 Hash: ed01ebfbc9eb5bbea545af4d01bf5f1071661840480439c6e5babe8e080e41aa

#Description
This project demonstrates malware traffic capture and analysis using:

- tcpdump
- Wireshark
- procwatch

## Files

capture.pcap – captured network traffic  
report.pdf – full analysis report 
strings_output.txt
floss_output.txt
ids_rules.txt – Snort IDS rules  
screenshots/ – screenshots of analysis


## IDS Rules

alert udp $HOME_NET any -> $EXTERNAL_NET 53 (msg:"Malware DNS Query"; sid:1000001; rev:1;)

alert tcp $HOME_NET any -> $EXTERNAL_NET 445 (msg:"Outbound SMB attempt"; sid:1000002; rev:1;)
