## nmap scanning network
```cmd
nmap -A -F -T1 10.10.10.223 -v 
nmap -A -F 10.10.10.233 -v
```
## ffuf 
```cmd
ffuf -w /usr/share/wordlists/dirb/common.txt -u http://tenet.htb/FUZZ -fc 403 -p 2
```
- secLists [https://github.com/danielmiessler/SecLists.git]
