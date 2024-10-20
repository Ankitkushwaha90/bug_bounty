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
```cmd
└─# shodan info       
Error: Please run "shodan init <api key>" before using this command
```
```cmd                                                                                                                                                           
┌──(root㉿kali)-[/home/ankit]
└─# shodan scan -h
Usage: shodan scan [OPTIONS] COMMAND [ARGS]...

  Scan an IP/ netblock using Shodan.

Options:
  -h, --help  Show this message and exit.

Commands:
  internet   Scan the Internet for a specific port and protocol using the...
  list       Show recently launched scans
  protocols  List the protocols that you can scan with using Shodan.
  status     Check the status of an on-demand scan.
  submit     Scan an IP/ netblock using Shodan.
```
```cmd
shodan count wordpress
521246
```
