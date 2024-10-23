- AtomDucky[https://github.com/FLOCK4H/AtomDucky.git]

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
```cmd
──(root㉿kali)-[/home/ankit]
└─# shodan host 98.137.11.163                  
98.137.11.163
Hostnames:               yahoo.com;ca.my.yahoo.com;hk.rd.yahoo.com;ddl.fp.yahoo.com;add.my.yahoo.com;ca.rogers.yahoo.com;mbp.yimg.com;tw.rd.yahoo.com;media-router-fp74.prod.media.vip.gq1.yahoo.com;fr-ca.rogers.yahoo.com;s.yimg.com;brb.yahoo.net
City:                    Quincy
Country:                 United States
Organization:            Oath Holdings Inc.
Updated:                 2024-10-22T14:39:19.379823
Number of open ports:    2

Ports:
     80/tcp  
        |-- HTTP title: Yahoo
    443/tcp  
        |-- HTTP title: Yahoo
        |-- Cert Issuer: C=US, OU=www.digicert.com, O=DigiCert Inc, CN=DigiCert SHA2 High Assurance Server CA
        |-- Cert Subject: C=US, ST=New York, CN=yahoo.com, O=Yahoo Holdings Inc., L=New York
        |-- SSL Versions: -SSLv2, -SSLv3, TLSv1, TLSv1.1, TLSv1.2, TLSv1.3

```
## theHarvester 
```cmd
┌──(root㉿kali)-[/home/ankit]
└─# theHarvester -d domain.com - go google.com
Created default proxies.yaml at /root/.theHarvester/proxies.yaml
*******************************************************************
*  _   _                                            _             *
* | |_| |__   ___    /\  /\__ _ _ ____   _____  ___| |_ ___ _ __  *
* | __|  _ \ / _ \  / /_/ / _` | '__\ \ / / _ \/ __| __/ _ \ '__| *
* | |_| | | |  __/ / __  / (_| | |   \ V /  __/\__ \ ||  __/ |    *
*  \__|_| |_|\___| \/ /_/ \__,_|_|    \_/ \___||___/\__\___|_|    *
*                                                                 *
* theHarvester 4.6.0                                              *
* Coded by Christian Martorella                                   *
* Edge-Security Research                                          *
* cmartorella@edge-security.com                                   *
*                                                                 *
*******************************************************************
usage: theHarvester [-h] -d DOMAIN [-l LIMIT] [-S START] [-p] [-s] [--screenshot SCREENSHOT] [-v] [-e DNS_SERVER] [-t] [-r [DNS_RESOLVE]] [-n] [-c] [-f FILENAME]
                    [-b SOURCE]
theHarvester: error: unrecognized arguments: - go google.com
                                                                                                                                                                      
┌──(root㉿kali)-[/home/ankit]
└─# 
```
