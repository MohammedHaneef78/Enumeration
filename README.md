# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain google.com

<img width="1901" height="968" alt="image" src="https://github.com/user-attachments/assets/e898194a-9b65-4b9b-8f36-047a8ccc38be" />



filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain google.com

<img width="1912" height="957" alt="image" src="https://github.com/user-attachments/assets/8572301c-a48c-4b7c-8b5d-bbb0269e547c" />




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1907" height="870" alt="image" src="https://github.com/user-attachments/assets/490c9631-db68-4620-85f5-7904dd0d050b" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="1897" height="962" alt="image" src="https://github.com/user-attachments/assets/795a99fc-e074-4833-8e96-9e89dd49d90e" />


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="1900" height="957" alt="image" src="https://github.com/user-attachments/assets/694e6d37-bc36-439e-b902-6d8eb2967152" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img width="1917" height="961" alt="image" src="https://github.com/user-attachments/assets/a842a3f9-7203-4f50-8ebb-8b95d1310f71" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

<img width="1375" height="777" alt="image" src="https://github.com/user-attachments/assets/b938409c-338a-462a-bf41-c464c3f39a43" />

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion


## OUTPUT:

<img width="1920" height="1080" alt="enumeration" src="https://github.com/user-attachments/assets/e130e260-746c-49b3-93c5-d4e2de40e7ff" />


##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

### Get the host’s addresses (A record):
```
dig google.com A
```


<img width="1920" height="923" alt="dig" src="https://github.com/user-attachments/assets/4d93884e-8844-4df9-89a4-360938512093" />

### Get the namservers (threaded):
```
dig google.com NS
```

<img width="1920" height="923" alt="threaded" src="https://github.com/user-attachments/assets/67fd2946-7dc5-44ee-bfa9-a3b30b91cace" />

### Get the MX record (threaded):
```
dig google.com MX
```

<img width="1920" height="923" alt="mx" src="https://github.com/user-attachments/assets/96a71b1a-c347-4fa7-ba9c-3ad418bfa911" />


### Perform axfr queries on nameservers and get BIND versions(threaded):
```

```
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

