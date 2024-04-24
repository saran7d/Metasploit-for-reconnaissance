# Metasploit-for-reconnaissance
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

- `Step 1:` Install kali linux either in partition or virtual box or in live mode

- `Step 2:` Investigate on the various categories of tools as follows:

- `Step 3:` Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system
![](1.PNG)

Invoke msfconsole
![](2.PNG)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.
![](3.png)

### Port scanning:
msf > nmap -sT 192.168.1810/24-p1-1000
![](4.png)

msf > db_nmap 192.168.181.0/24
![](5.png)

kali > ls-l
![](6.png)

search
![](7.PNG)

info
![](8.PNG)

### MYSQL ENUMERATION
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
![](9.PNG)

search
![](10.PNG)

use 11 Or: use auxiliary/scanner/mysql/mysql_version
![](11.PNG)

Use the set rhosts command to set the parameter and run the module, as follows:
![](12.PNG)

After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module
![](13.PNG)

/usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt
![](14.PNG)

![](15.PNG)
## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
